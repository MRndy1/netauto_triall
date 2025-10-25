# netauto_trial

# Network Configuration Automation Tool

This project automates checking and applying network configuration changes.

## Run
```bash
python -m src.main verify --config data/running_config_before.txt --topology_or_changes changes/changes.yaml
python -m src.main apply --config data/running_config_before.txt --changes changes/changes.yaml --out data/running_config_after.txt
python -m src.main verify --config data/running_config_after.txt --topology_or_changes changes/changes.yaml

