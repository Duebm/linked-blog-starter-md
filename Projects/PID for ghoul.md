Would need balloon sim
- Matlab
- Tune to flight logs of accent rate

[GHOUL/pid_sim/Simulation/sim.c at main · UMDBPP/GHOUL · GitHub](https://github.com/UMDBPP/GHOUL/blob/main/pid_sim/Simulation/sim.c)


%% Load Balloon Flight Log

filename = '025.csv';

% Read as table for easy column access

rawLines = readlines(filename);

splitData = split(rawLines, ",");

T = array2table(splitData);

commasthere = 12;

% Fix for weirdness

T(:,2:commasthere) = [];

% Headers

headers = matlab.lang.makeValidName(T{1,:});

T.Properties.VariableNames = headers;

T(1,:) = [];

head(T,10)

% Extract relevant fields

Time_s_ = T(:,1);

Alt_m_= T(:,11);

aRate_m_s_= T(:,15);

T.Time_s_ = str2double(T.Time_s_);

T.aRate_m_s_ = str2double(T.aRate_m_s_);

T.Alt_m_ = str2double(T.Alt_m_);

% %% Quick Plot of Actual Flight Profile

% figure;

% plot(T.Time_s_, T.Alt_m_, 'LineWidth', 2);

% %xlabel('Time (s)'); ylabel('Altitude (m)');

% %title('Actual Balloon Flight Altitude vs Time');

%

% figure;

% plot(T.Time_s_, T.aRate_m_s_, 'LineWidth', 2);

% %xlabel('Time (s)'); ylabel('Vertical Speed (m/s)');

% %title('Vertical Speed Profile');