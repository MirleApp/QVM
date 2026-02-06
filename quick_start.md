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

### Start QVM Trial Version

```bash
sudo docker load -i miqvm-trial.tar
sudo docker compose -f docker-compose-all-in-one.yml up -d
```

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