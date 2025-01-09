## Driving Simulator Telemetry - MQTT Topics
Here you will find an overview of all telemetry data published by the driving simulator via MQTT:

### Race
| Topic                                 | Example Value          |
|---------------------------------------|------------------------|
| Sim1/Race/Data/InRace                 | True                   |
| Sim1/Race/Data/GameName               | Project Cars 2         |
| Sim1/Race/Data/CarName                | Porsche 919 Hybrid     |
| Sim1/Race/Data/TrackName              | Nurburgring            |
| Sim1/Race/Data/Lap                    | 3                      |
| Sim1/Race/Data/CurrentLapTime         | 99.99829               |
| Sim1/Race/Data/BestLapTime            | 398.01025              |
| Sim1/Race/Data/LastLapTime            | 398.01025              |
| Sim1/Race/Data/Position               | 0                      |
| Sim1/Race/Data/TotalPositions         | 0                      |
| Sim1/Race/Data/Coordinate/0           | 0                      |
| Sim1/Race/Data/Coordinate/1           | 0                      |
| Sim1/Race/Data/Coordinate/2           | 0                      |


### Car
| Topic                                 | Example Value          |
|---------------------------------------|------------------------|
| Sim1/Car/Data/EngineActive            | True                   |
| Sim1/Car/Data/ESPActive               | False                  |
| Sim1/Car/Data/ABSActive               | False                  |
| Sim1/Car/Data/TCActive                | False                  |
| Sim1/Car/Data/Light                   | False                  |
| Sim1/Car/Data/Fullbeam                | False                  |
| Sim1/Car/Data/Indicators/0            | False                  |
| Sim1/Car/Data/Indicators/1            | False                  |
| Sim1/Car/Data/Throttle                | 99                     |
| Sim1/Car/Data/Brake                   | 99                     |
| Sim1/Car/Data/Steering                | 99                     |
| Sim1/Car/Data/Clutch                  | 98                     |
| Sim1/Car/Data/FuelCapacity            | 62                     |
| Sim1/Car/Data/FuelLevel               | 1                      |
| Sim1/Car/Data/FuelPressure            | 0.58                   |
| Sim1/Car/Data/WaterPressure           | 2.76                   |
| Sim1/Car/Data/WaterTemp               | 99                     |
| Sim1/Car/Data/Speed                   | 99.99                  |
| Sim1/Car/Data/RPM                     | 999                    |
| Sim1/Car/Data/MaxRPM                  | 8500                   |
| Sim1/Car/Data/Gear                    | 7                      |
| Sim1/Car/Data/OdometerKM              | 9.999                  |
| Sim1/Car/Data/OilPressure             | 4.82                   |
| Sim1/Car/Data/OilTemp                 | 99                     |
| Sim1/Car/Data/Orientation/0           | 0.174                  |
| Sim1/Car/Data/Orientation/1           | 3.142                  |
| Sim1/Car/Data/Orientation/2           | 0.237                  |
| Sim1/Car/Data/LocalVelocity/0         | 9.97                   |
| Sim1/Car/Data/LocalVelocity/1         | 3.156                  |
| Sim1/Car/Data/LocalVelocity/2         | 9.983                  |
| Sim1/Car/Data/WorldVelocity/0         | 9.999                  |
| Sim1/Car/Data/WorldVelocity/1         | 9.96                   |
| Sim1/Car/Data/WorldVelocity/2         | 9.999                  |
| Sim1/Car/Data/AngularVelocity/0       | 1.929                  |
| Sim1/Car/Data/AngularVelocity/1       | 6.899                  |
| Sim1/Car/Data/AngularVelocity/2       | 3.105                  |
| Sim1/Car/Data/LocalAcceleration/0     | 94.764                 |
| Sim1/Car/Data/LocalAcceleration/1     | 99.438                 |
| Sim1/Car/Data/LocalAcceleration/2     | 92.34                  |
| Sim1/Car/Data/WorldAcceleration/0     | 92.794                 |
| Sim1/Car/Data/WorldAcceleration/1     | 97.197                 |
| Sim1/Car/Data/WorldAcceleration/2     | 98.759                 |
| Sim1/Car/Data/ExtentsCentre/0         | 0                      |
| Sim1/Car/Data/ExtentsCentre/1         | 0.583                  |
| Sim1/Car/Data/ExtentsCentre/2         | -0.065                 |
| Sim1/Car/Data/TyreY/0                 | 0.038                  |
| Sim1/Car/Data/TyreY/1                 | 0.038                  |
| Sim1/Car/Data/TyreY/2                 | 0.058                  |
| Sim1/Car/Data/TyreY/3                 | 0.059                  |
| Sim1/Car/Data/TyreRPS/0               | 9.985                  |
| Sim1/Car/Data/TyreRPS/1               | 9.985                  |
| Sim1/Car/Data/TyreRPS/2               | 9.998                  |
| Sim1/Car/Data/TyreRPS/3               | 9.99                   |
| Sim1/Car/Data/TyreTemp/0              | 99                     |
| Sim1/Car/Data/TyreTemp/1              | 96                     |
| Sim1/Car/Data/TyreTemp/2              | 99                     |
| Sim1/Car/Data/TyreTemp/3              | 94                     |
| Sim1/Car/Data/TyreHeightAboveGround/0 | 0.465                  |
| Sim1/Car/Data/TyreHeightAboveGround/1 | 0.386                  |
| Sim1/Car/Data/TyreHeightAboveGround/2 | 0.443                  |
| Sim1/Car/Data/TyreHeightAboveGround/3 | 0.355                  |
| Sim1/Car/Data/TyreWear/0              | 9                      |
| Sim1/Car/Data/TyreWear/1              | 9                      |
| Sim1/Car/Data/TyreWear/2              | 9                      |
| Sim1/Car/Data/TyreWear/3              | 9                      |
| Sim1/Car/Data/BrakeDamage/0           | 0                      |
| Sim1/Car/Data/BrakeDamage/1           | 0                      |
| Sim1/Car/Data/BrakeDamage/2           | 0                      |
| Sim1/Car/Data/BrakeDamage/3           | 0                      |
| Sim1/Car/Data/SuspensionDamage/0      | 0                      |
| Sim1/Car/Data/SuspensionDamage/1      | 0                      |
| Sim1/Car/Data/SuspensionDamage/2      | 0                      |
| Sim1/Car/Data/SuspensionDamage/3      | 0                      |
| Sim1/Car/Data/BrakeTempCelsius/0      | 999                    |
| Sim1/Car/Data/BrakeTempCelsius/1      | 999                    |
| Sim1/Car/Data/BrakeTempCelsius/2      | 761                    |
| Sim1/Car/Data/BrakeTempCelsius/3      | 778                    |
| Sim1/Car/Data/TyreTreadTemp/0         | 99                     |
| Sim1/Car/Data/TyreTreadTemp/1         | 95                     |
| Sim1/Car/Data/TyreTreadTemp/2         | 99                     |
| Sim1/Car/Data/TyreTreadTemp/3         | 93                     |
| Sim1/Car/Data/TyreLayerTemp/0         | 99                     |
| Sim1/Car/Data/TyreLayerTemp/1         | 99                     |
| Sim1/Car/Data/TyreLayerTemp/2         | 99                     |
| Sim1/Car/Data/TyreLayerTemp/3         | 99                     |
| Sim1/Car/Data/TyreCarcassTemp/0       | 99                     |
| Sim1/Car/Data/TyreCarcassTemp/1       | 99                     |
| Sim1/Car/Data/TyreCarcassTemp/2       | 99                     |
| Sim1/Car/Data/TyreCarcassTemp/3       | 99                     |
| Sim1/Car/Data/TyreRimTemp/0           | 99                     |
| Sim1/Car/Data/TyreRimTemp/1           | 99                     |
| Sim1/Car/Data/TyreRimTemp/2           | 99                     |
| Sim1/Car/Data/TyreRimTemp/3           | 99                     |
| Sim1/Car/Data/TyreInternalAirTemp/0   | 99                     |
| Sim1/Car/Data/TyreInternalAirTemp/1   | 99                     |
| Sim1/Car/Data/TyreInternalAirTemp/2   | 99                     |
| Sim1/Car/Data/TyreInternalAirTemp/3   | 99                     |
| Sim1/Car/Data/TyreTempLeft/0          | 99                     |
| Sim1/Car/Data/TyreTempLeft/1          | 98                     |
| Sim1/Car/Data/TyreTempLeft/2          | 99                     |
| Sim1/Car/Data/TyreTempLeft/3          | 99                     |
| Sim1/Car/Data/TyreTempCenter/0        | 99                     |
| Sim1/Car/Data/TyreTempCenter/1        | 96                     |
| Sim1/Car/Data/TyreTempCenter/2        | 99                     |
| Sim1/Car/Data/TyreTempCenter/3        | 94                     |
| Sim1/Car/Data/TyreTempRight/0         | 99                     |
| Sim1/Car/Data/TyreTempRight/1         | 94                     |
| Sim1/Car/Data/TyreTempRight/2         | 99                     |
| Sim1/Car/Data/TyreTempRight/3         | 92                     |
| Sim1/Car/Data/WheelLocalPositionY/0   | 0.054                  |
| Sim1/Car/Data/WheelLocalPositionY/1   | 0.053                  |
| Sim1/Car/Data/WheelLocalPositionY/2   | 0.055                  |
| Sim1/Car/Data/WheelLocalPositionY/3   | 0.051                  |
| Sim1/Car/Data/RideHeight/0            | 0.2                    |
| Sim1/Car/Data/RideHeight/1            | 0.2                    |
| Sim1/Car/Data/RideHeight/2            | 0.2                    |
| Sim1/Car/Data/RideHeight/3            | 0.2                    |
| Sim1/Car/Data/SuspensionTravel/0      | 0.029                  |
| Sim1/Car/Data/SuspensionTravel/1      | 0.034                  |
| Sim1/Car/Data/SuspensionTravel/2      | 0.045                  |
| Sim1/Car/Data/SuspensionTravel/3      | 0.036                  |
| Sim1/Car/Data/SuspensionVelocity/0    | 1.91                   |
| Sim1/Car/Data/SuspensionVelocity/1    | 1.847                  |
| Sim1/Car/Data/SuspensionVelocity/2    | 3.032                  |
| Sim1/Car/Data/SuspensionVelocity/3    | 1.723                  |
| Sim1/Car/Data/AirPressure/0           | 2.01                   |
| Sim1/Car/Data/AirPressure/1           | 1.99                   |
| Sim1/Car/Data/AirPressure/2           | 1.92                   |
| Sim1/Car/Data/AirPressure/3           | 1.91                   |
| Sim1/Car/Data/EngineSpeed             | 99                     |
| Sim1/Car/Data/EngineTorque            | 999.851                |
| Sim1/Car/Data/HandBrake               | 0                      |
| Sim1/Car/Data/AeroDamage              | 0                      |
| Sim1/Car/Data/EngineDamage            | 0                      |
| Sim1/Car/Data/AmbientTemperature      | 23                     |
| Sim1/Car/Data/TrackTemperature        | 34                     |
| Sim1/Car/Data/RainDensity             | 0                      |
| Sim1/Car/Data/SnowDensity             | 0                      |
| Sim1/Car/Data/WindSpeed               | 0                      |
| Sim1/Car/Data/WindDirectionX          | 98                     |
| Sim1/Car/Data/WindDirectionY          | 33                     |
| Sim1/Car/Data/CurrentRealTime         | 2024-11-20 13:22:32:48 |



