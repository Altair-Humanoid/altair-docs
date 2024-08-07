# Robot Tuning

<aside>
💡 Make Sure to **Fasten Every Joint Bolts** Before Tuning

</aside>

> **Coordinate Guides:**
> 
> 
> **X**: Front Back Axis
> 
> **Y**: Up Down Axis
> 
> **Z**: Right Left Axis
> 

> **Shift** untuk pusat massa(pm) torso(badan)
> 
> 
> **Lift** untuk posisi akhir kaki ketika mengangkat
> 
> **Swing** untuk posisi akhir kaki ketika menendang
> 
> **Retract** untuk posisi akhir kaki ketika menarik
> 

## kicking_v10:

```yaml
  Torso_X: 0.02 #[0.0015] Posisi Awal dan Akhir Torso sumbu X {-0.0015}
  Torso_Y: 0.0 #Posisi Awal dan Akhir Torso sumbu Y {0.0}
  Torso_Z: 0.3450 #Tinggi Torso Awal dan Akhir {0.3450}
#Ketika menendang Kaki Kiri
  L_Shift_X: 0.005 #Posisi Torso ketika shifting Sumbu X
  L_Shift_Y: -0.095 #Posisi Torso ketika shifting Sumbu Y
  L_Shift_Z: 0.353 #Tinggi Torso ketika shifting
#Ketika menendang Kaki Kanan
  R_Shift_X: 0.040 # [0.027] Posisi Torso ketika shifting Sumbu X {0.0}
  R_Shift_Y: 0.096 # [0.095] Posisi Torso ketika shifting Sumbu X {0.075} {0.1} {0.096}
  R_Shift_Z: 0.360 # Posisi Torso ketika shifting Sumbu X {0.360} {0.355}
#Ketika menendang Kaki Kiri
  L_Lift_X: -0.12 #Posisi Kaki kiri ketika mengangkat pada Sumbu X
  L_Lift_Y: 0.07 #Posisi Kaki kiri ketika mengangkat pada Sumbu Y
  L_Lift_Z: 0.1 #Posisi Kaki kiri ketika mengangkat pada Sumbu Z
#Ketika menendang Kaki Kanan
  R_Lift_X: -0.13 #Posisi akhir Kaki kanan ketika mengangkat pada Sumbu X {-0.12}
  R_Lift_Y: -0.05 #Posisi akhir Kaki kanan ketika mengangkat pada Sumbu Y {-0.07}
  R_Lift_Z: 0.14 #Posisi akhir Kaki kanan ketika mengangkat pada Sumbu Z {0.17}
#Ketika menendang Kaki Kiri
  L_Swing_X: 0.3 #Posisi akhir Kaki kiri ketika menendang pada Sumbu X
  L_Swing_Y: 0.07 #Posisi akhir Kaki kiri ketika menendang pada Sumbu Y
  L_Swing_Z: 0.08 #Posisi akhir Kaki kiri ketika menendang pada Sumbu Z
#Ketika menendang Kaki Kanan
  R_Swing_X: 0.25 #Posisi akhir Kaki kanan ketika menendang pada Sumbu X {0.31}
  R_Swing_Y: -0.05 #Posisi akhir Kaki kanan ketika menendang pada Sumbu Y {-0.07}
  R_Swing_Z: 0.15 #Posisi akhir Kaki kanan ketika menendang pada Sumbu Z {0.14}
#Ketika menarik setelah menendang Kaki Kiri
  L_Retract_X: 0.0 #Posisi akhir Kaki kiri ketika menarik pada Sumbu X
  L_Retract_Y: 0.1 #Posisi akhir Kaki kiri ketika menarik pada Sumbu Y
  L_Retract_Z: 0.1 #Posisi akhir Kaki kiri ketika menarik pada Sumbu Z
#Ketika menarik setelah menendang Kaki Kanan
  R_Retract_X: 0.05 #Posisi akhir Kaki kanan ketika menarik pada Sumbu X {0.0}
  R_Retract_Y: -0.06 #Posisi akhir Kaki kanan ketika menarik pada Sumbu Y {-0.1}
  R_Retract_Z: 0.14 #[0.11] Posisi akhir Kaki kanan ketika menarik pada Sumbu Z {0.17}

#Sudut
  Shift_Roll: 16.0 # [16.5] Posisi Trunk Roll ketika shifting {15.0}
  Torso_Pitch: 5.0 #[12.5] Posisi Trunk Pitch ketika awal dan akhir {5.0}
  Lift_Roll: 25.0 # [27.5] Posisi Trunk Roll ketika Lift {25.0}
  Lift_Pitch: 10.0 # [28.5] Posisi Trunk Pitch ketika Lift {5.0}
  Swing_Roll: 25.0 # [27.5] Posisi Trunk Roll ketika Swing {25.0}
  Swing_Pitch: 10.0 # [28.5] Posisi Trunk Pitch ketika Swing{5.0}
  Retract_Roll: 16.5 # [16.5] Posisi Trunk Roll ketika Retract {14.00} {16.5]
  Retract_Pitch: 5.5 #[15.0]Posisi Trunk Pitch ketika Retract {5.5}

##Timing
  SHIFT_TIME: 1.2 ##Waktu untuk shifting dalam second {1.2}
  LIFT_TIME: 0.24 ##Waktu untuk lifting dalam second {0.3}
  SWING_TIME: 0.24 ##Waktu untuk swing dalam second {0.3}
  RETRACT_TIME: 0.15 ##Waktu untuk retract dalam second {0.15}
  LANDING_TIME: 0.15 ##Waktu untuk landing dalam second {0.15}
  FINISHED_TIME: 0.2 ##Waktu untuk pause setelah menendang dalam second {0.2}

reference dari robotis op3
https://emanual.robotis.com/docs/en/platform/op3/robotis_ros_packages/ 
```