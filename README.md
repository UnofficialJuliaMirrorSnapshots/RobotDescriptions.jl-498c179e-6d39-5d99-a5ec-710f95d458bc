# RobotDescriptions

[![Build Status](https://travis-ci.org/phelipe/RobotDescriptions.jl.svg?branch=master)](https://travis-ci.org/phelipe/RobotDescriptions.jl)

This small package provides URDF and meshes for robots, as well as a convenience function for creating a RigidBodyDynamics.Mechanism.

### Install

```julia
(v1.0) pkg> add https://github.com/phelipe/RobotDescriptions.jl
```



### Usage
- Get a `RigidBodyDynamics.Mechanism` of a robot. 
```julia
julia> robot =  getmechanism("kukalwr")
```

- Get a `MechanismGeometries.URDF.URDFVisuals` of a robot.
```julia
julia> visual = getvisual("kukalwr")
```
- Get a `RigidBodyDynamics.Mechanism` and `MechanismGeometries.URDF.URDFVisuals` of a robot.
```julia
julia> robot, visual = getrobot("kukalwr")
```



### Robotss

Robot | name
------------ | -------------
Universal robot ur5 | ur5
Generic Acrobot | acrobot
KUKA LWR 4 + | kuka-lwr-4plus
PUMA 560 | puma560
DENSO VS -060 | denso060