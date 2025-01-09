# Grafana Workshop

This repository provides the materials for the workshop *Grafana & Co: Visualization and monitoring of time series data with Grafana, Telegraf and InfluxDB*.

Please download or clone this repository to join the workshop.

## Commands
Start and run the TIG-stack defined in [tig-stack/docker-compose.yaml](tig-stack/docker-compose.yaml):

```bash
cd tig-stack
docker compose up
```

Restart the Telegraf agent after changes to its configuration.

```bash
docker compose restart telegraf
```

## Web-Interfaces

[InfluxDB http://localhost:8086](http://localhost:8086)

[Grafana http://localhost:3000](http://localhost:3000)


## Selection of MQTT Topics

A selection of published MQTT topics for a Telegraf configuration:
```bash
  topics = [
    "Sim1/Car/Data/Throttle",
    "Sim1/Car/Data/Brake",
    "Sim1/Car/Data/Steering",
    "Sim1/Car/Data/Clutch",
    "Sim1/Car/Data/FuelLevel",
    "Sim1/Car/Data/FuelPressure",
    "Sim1/Car/Data/WaterPressure",
    "Sim1/Car/Data/WaterTemp",
    "Sim1/Car/Data/Speed",
    "Sim1/Car/Data/RPM",
    "Sim1/Car/Data/Gear",
    "Sim1/Car/Data/OdometerKM",
    "Sim1/Car/Data/OilPressure",
    "Sim1/Car/Data/OilTemp",
    "Sim1/Car/Data/Orientation/0",
    "Sim1/Car/Data/Orientation/1",
    "Sim1/Car/Data/Orientation/2",
    "Sim1/Car/Data/WorldAcceleration/0",
    "Sim1/Car/Data/WorldAcceleration/1",
    "Sim1/Car/Data/WorldAcceleration/2",

    "Sim1/Car/Data/TyreRPS/0",
    "Sim1/Car/Data/TyreRPS/1",
    "Sim1/Car/Data/TyreRPS/2",
    "Sim1/Car/Data/TyreRPS/3",
    "Sim1/Car/Data/TyreTemp/0",
    "Sim1/Car/Data/TyreTemp/1",
    "Sim1/Car/Data/TyreTemp/2",
    "Sim1/Car/Data/TyreTemp/3",

    "Sim1/Car/Data/BrakeTempCelsius/0",
    "Sim1/Car/Data/BrakeTempCelsius/1",
    "Sim1/Car/Data/BrakeTempCelsius/2",
    "Sim1/Car/Data/BrakeTempCelsius/3",
    
    "Sim1/Car/Data/AirPressure/0",
    "Sim1/Car/Data/AirPressure/1",
    "Sim1/Car/Data/AirPressure/2",
    "Sim1/Car/Data/AirPressure/3",
    "Sim1/Car/Data/EngineSpeed",
    "Sim1/Car/Data/EngineTorque",

    "Sim1/Race/Data/Lap",
    "Sim1/Race/Data/CurrentLapTime",
    "Sim1/Race/Data/BestLapTime",
    "Sim1/Race/Data/TrackName",
    "Sim1/Race/Data/CarName"
  ]
```

## All MQTT Topics
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



## Dashboard Scenarios

#### 1. Vehicle Performance 

This dashboard focuses on the core performance metrics of the car.

 1.	Speed (Speed): Line chart showing the car’s speed over time.
 2.	Engine RPM (RPM): Line chart comparing the current RPM with the gear position (Gear).
 3.	Throttle Position (Throttle): Chart showing the throttle usage.
 4.	Brake Pedal Position (Brake): Visualizing brake activity.
 5.	Engine Torque (EngineTorque): Displaying the engine’s generated torque.
 6.	Odometer (OdometerKM): Graph showing the distance traveled.
 7.	Gear: Panel showing the current gear.


#### 2. Race Statistics 

This dashboard provides an overview of the car’s racing performance.

1. Current Lap Time (CurrentLapTime): line chart showing the current lap time.
2. Best Lap Time (BestLapTime): SingleStat displaying the best lap time achieved.
3. Current Lap Number (Lap): gauge panel visualizing the current lap count.
4. Speed (Speed): chart showing speed trends during the race.
5. Engine RPM (RPM): chart correlating RPM with other metrics like speed.
6. Track Name (TrackName): text panel showing the current track name.


#### 3. Engine and Fluid Monitoring 

This dashboard focuses on monitoring fluid levels and temperatures.

1. Fuel Level (FuelLevel):  chart showing the remaining fuel in the tank
2. Fuel Pressure (FuelPressure): chart visualizing fuel system pressure.
3. Water Temperature (WaterTemp): chart showing engine cooling performance.
4. Oil Pressure (OilPressure): chart monitoring oil pressure levels.
5. Oil Temperature (OilTemp): chart visualizing oil temperature.
6. Water Pressure (WaterPressure): chart displaying water pressure in the system.


#### 4. Tire and Brake Monitoring 

This dashboard monitors the tires and brakes of the car.

1. Tire Temperature (TyreTemp for all wheels): Heatmap showing temperature distribution across all tires.
2. Tire Revolutions Per Second (TyreRPS for all wheels): Line chart showing tire rotation speeds.
3. Brake Temperature (BrakeTempCelsius for all wheels): chart visualizing brake temperatures.
4. Tire Air Pressure (AirPressure for all wheels): chart showing air pressure in the tires.
5. Front vs. Rear Tires (Temperature): comparison chart highlighting temperature differences between front and rear tires.
6. Brake Temperature Overview: Gauge panel warning of critical brake temperatures.


#### 5. Vehicle Dynamics 

This dashboard provides insights into the car’s dynamics while in motion.

1. Acceleration (WorldAcceleration): chart displaying acceleration values in X, Y, and Z directions.
2. Steering Input (Steering): chart visualizing steering inputs over time.
3. Orientation (Orientation in X, Y, Z): visualization showing the car’s orientation.
4. Clutch Position (Clutch): chart showing clutch usage over time.
5. Engine Speed (EngineSpeed): chart correlating engine speed with acceleration.
6. Environmental Conditions: displays ambient and track temperatures (AmbientTemperature, TrackTemperature).
7. Speed (Speed): chart showing speed trends during the race.



## Helpful Links

### Telegraf
[Telegraf Documentation](https://docs.influxdata.com/telegraf/latest/)

[Telegraf Image on Docker Hub](https://hub.docker.com/_/telegraf)

[Telegraf Plugins](https://github.com/influxdata/telegraf/tree/master/plugins)

### Grafana
[Grafana Documentation](https://grafana.com/docs)

[Grafana Image on Docker Hub](https://hub.docker.com/r/grafana/grafana)


### InfluxDB
[InfluxDB Documentation](https://docs.influxdata.com/telegraf/latest/)

[InfluxDB Image on Docker Hub](https://hub.docker.com/_/influxdb)

