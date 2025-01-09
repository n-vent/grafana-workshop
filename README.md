# Grafana Workshop

This repository provides the materials for the workshop *Grafana & Co: Visualization and monitoring of time series data with Grafana, Telegraf and InfluxDB*.

Please download or clone this repository to participate in the workshop.

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

The web interfaces of the TIG-stack can be accessed via the following ports:

[InfluxDB http://localhost:8086](http://localhost:8086)

[Grafana http://localhost:3000](http://localhost:3000)


## Selection of MQTT Topics

You can find a complete overview of all telemetry data published by the driving simulator via MQTT in [Sim1-MQTT-Topics.md](Sim1-MQTT-Topics.md)

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

