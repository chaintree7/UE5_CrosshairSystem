
# Advanced Crosshair System
### This is a very easy to integrate component that will easily add a precise crosshair to your project and you can also add unique properties for each weapon


---

### Usage: Just add component `CT_Cmpt_Crosshair` to your Actor.
![image](https://github.com/user-attachments/assets/81f58f80-e902-4a6e-bedd-c61ecfc343f3)

## Component Parameters
![image](https://github.com/user-attachments/assets/f5f932e6-e4a3-4533-8933-7e3fd494711e)



| Params| Description |
| ----------- | ----------- |
| `Widget Class` |  `Crosshair UI Widget Class` 
| `Base Spread` |  `The base spread` 
| `Jump Spread` |  `Additional spread when jumping or falling` 
| `Movement Spread` |  `Additional spread when moving` 
| `Max Spread` |  `The maximum spread`
| `Spread Recovery Time Curve` |  `Spread Recovery Time Curve (Usually just use the default curve)` 
| `Spread Recovery Rate` |  `Spread Recovery Rate` 
| `Correction Factor` |  `When line trace, the impact point will be offset depending on the start point.(3000 for start point is Actor position)` 
---
# Functions

## Crosshair Widget
#### Show and hide the Crosshair. For example, hide when unarmed and show when switching to guns.
![image](https://github.com/user-attachments/assets/58e1ca83-6a76-4651-bb64-0304324c8024)

## Add Dynamic Spread
#### Temporarily increases the spread when firing. The temporary spread will automatically recover to 0. The Recovery Rate affects the speed of recovery.
![image](https://github.com/user-attachments/assets/07972668-419e-4063-8591-a7ad68ee7662)


## Line Trace ***
#### Line trace based on the current spread.
![image](https://github.com/user-attachments/assets/9b23c971-e7e4-4a7a-b394-3d47e17aec6a)

| Params| Description |
| ----------- | ----------- |
| `Start Point` |  `e.g. use camera position. If this Character (Actor) is AI, use the Actor position` 
| `Distance` |  `Firing range` 

## Set Default Spread
#### Changing default parameters
![image](https://github.com/user-attachments/assets/f2083d72-a668-4426-8ade-a48eb0db497b)

| Params| Description |
| ----------- | ----------- |
| `Base` |  `Base Spread` 
| `Jump` |  `Jump Spread` 
| `Movement` |  `Movement Spread` 
| `Max` |  `Max Spread` 

## Get Spread Value
#### Get the current spread value.
![image](https://github.com/user-attachments/assets/5706598d-518a-4aff-8fe6-b2c03482626e)

## Event OnSpreadChanged
![image](https://github.com/user-attachments/assets/8f5acbf0-90be-4c38-9ab4-b154a36e5114)

