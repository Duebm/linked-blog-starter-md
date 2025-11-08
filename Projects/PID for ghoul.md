Would need balloon sim
- Matlab
- Tune to flight logs of accent rate


%% Load Balloon Flight Log

filename = '025.csv';

% Read as table for easy column access

T = readtable(filename);

print (T)

% % Extract relevant fields

% time = T.Time_s_; % seconds since launch

% alt = T.Alt_m_; % altitude (m)

% vz = T.aRate_m_s_; % vertical velocity (m/s)

% pres = Pres_hPa_; % pressure (hPa)

%

% %% Quick Plot of Actual Flight Profile

% figure;

% plot(time, alt, 'LineWidth', 2);

% xlabel('Time (s)'); ylabel('Altitude (m)');

% title('Actual Balloon Flight Altitude vs Time');

%

% figure;

% plot(time, vz, 'LineWidth', 2);

% xlabel('Time (s)'); ylabel('Vertical Speed (m/s)');

% title('Vertical Speed Profile');