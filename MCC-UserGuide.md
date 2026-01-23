# MCC User Guide

Enter the MCC system URL in the address bar and open the MCC website to access the main page.
![MCC Main Page](mcc_user_guide_images/2-02_home.png)

---

## Data Collection

Select production history conditions within a time range for modeling, and click Get Piece to retrieve the number of data records for modeling.

![MCC Modeling Data Filtering Page](mcc_user_guide_images/2-03_modeling_data_filtering.png)
 
Click Piece Count to display the Piece ID list, where you can select or exclude Piece IDs. Finally, click Next to proceed to the data parameter filtering step.

![Click Piece Count](mcc_user_guide_images/2-04_click_piece_count.png)

![Piece ID List](mcc_user_guide_images/2-05_piece_id_list.png)

---

## Data Parameter Filtering

Select important production parameters and measurement types to include in the modeling model. After selection, click Next to proceed to the data preprocessing step.

![MCC Data Parameter Filtering Page](mcc_user_guide_images/2-06_data_parameter_filtering.png)

---

## Data Preprocessing

Set specifications for each important parameter and configure upper and lower limits (USL, LSL, UCL, LCL) through algorithms.

![MCC Setting Important Parameter Specifications Page](mcc_user_guide_images/2-07_setting_important_parameter_specifications.png)

Display data for a single important parameter.

![MCC Display Single Parameter Data Page](mcc_user_guide_images/2-08_display_single_parameter_data.png)

Display trend chart for a single important parameter.

![MCC Display Single Parameter Trend Page](mcc_user_guide_images/2-09_displays_a_single_parameter_trend.png)

---

## Algorithm Parameter Configuration

Algorithm parameter terminology explanation

| System | Term | Description |
|------|------|------|
| **Metrology Setting** | Target | Specification target |
| | USL | Upper specification limit |
| | LSL | Lower specification limit |
| | UCL | Upper control limit |
| | LCL | Lower control limit |
| **DOI<sub>k</sub> Model** | PhaseI Error Threshold | Maximum allowable error threshold between actual measurement and predicted values |
| **Neuro Network(NN) Model** | Mom Term Range | Momentum term<br>Direction of steepest descent of instantaneous error plus a proportion of the previous iteration adjustment value.<br>Learning rate of the inertia factor; larger values result in slower learning rates. |
| | Alpha Range | Learning rate<br>Smaller values: slower convergence process but relatively higher iteration count; Larger values: accelerate search efficiency but may cause unstable oscillations in the objective function during the search process. |
| | Epochs Range | Iteration count limit<br>Larger values result in more iterations (loops) |
| | Nodes Range | Number of neurons |
| **Reliable Index(RI) Model** | Tolerable Maximum Error | Maximum allowable error threshold for NN and PLS predicted values |

After configuration is complete, click Build to create the model

![MCC Algorithm Configuration Page](mcc_user_guide_images/2-10_algorithm_settings.png)