# MI-QVM Trial Version Operation Flow

* **Launch**
    * Obtain Image
    * Start QVM Trial Version

* **Operation**
    * Visit QVM Trial Version Page
    * Create Dataset
    * Operate MCC Modeling
    * Download Report
    * Open Report

## Launch

### Obtain Image

![Obtain Image](quick_start_images/get_image.png)

### Start QVM Trial Version

```bash
sudo docker load -i combined-backup.tar
sudo docker run -d --name combined-api -p 5500:5500 -p 9999:7878 combined-api-image:latest
```

![Start QVM Trial Version](quick_start_images/docker_run.png)

## Operation

### Visit QVM Trial Version Page

Access the following URL:
http://127.0.0.1:9999/trial

![Visit QVM Trial Version Page](quick_start_images/qvm_trial.png)

### Create Dataset


![Create Dataset](quick_start_images/create_dataset.png) <img src="quick_start_images/csvs.png" width="300" alt="CSVs" /> 
### CSV Content Reference

![CSV Content Reference](quick_start_images/op.png)

### Operate MCC Modeling

![Operate MCC Modeling](quick_start_images/op2.png)

### Download Report

![Download Report](quick_start_images/done.png)

### Open Report

![Open Report](quick_start_images/report.png)