
# Assignment-8

## 1. Schedule a Daily Backup of VM at 3:00 AM using Vault

### Resources
- [YouTube Video](https://www.youtube.com/watch?v=IzV03NqMnTE)
- [Microsoft Learn](https://learn.microsoft.com/en-us/training/paths/azure-administrator-monitor-backup-resources/)

### Steps
1. **Create a Recovery Services Vault**:
    - Sign in to the [Azure portal](https://portal.azure.com/)
    - Create a resource and search for "Backup and Site Recovery (OMS)".
    - Configure the vault with a unique name, subscription, resource group, and location.
    - Review and create the vault.

2. **Configure Backup for the VM**:
    - Navigate to the Recovery Services vault.
    - Click on Backup under Getting Started.
    - Set workload running in Azure and backup for Virtual machine.

3. **Create a Backup Policy**:
    - Create a new backup policy.
    - Set the policy name, backup frequency to daily at 3:00 AM, and retention range to 30 days.

4. **Apply the Backup Policy to the VM**:
    - Select the VM(s) to back up.
    - Click Enable Backup.

5. **Verify Backup Configuration**:
    - Go to Protected Items under the Recovery Services vault.
    - Ensure the VM is listed with the applied backup policy.

## 2. Create an Alert Rule for VM CPU Percentage

### Steps
1. **Navigate to Azure Monitor**:
    - In the Azure portal, navigate to Monitor.

2. **Create an Alert Rule**:
    - Click on Alerts, then New Alert Rule.
    - Select the VM resource to monitor.
    - Add a condition, selecting the metric "CPU Percentage".
    - Set the criteria to "Greater than" 80%.
    - Configure action groups to send email notifications.
    - Define the alert rule details and create the alert rule.
  3. **Now its done**    

## 3. Provision Backups in Backup Center

### Steps
1. **Navigate to Backup Center**:
    - In the Azure portal, navigate to Backup Center.

2. **Provision Backups**:
    - Click on +Backup to start the backup provisioning process.
    - Select the appropriate backup goal and follow the prompts to configure backups for your resources.

## 4. Schedule a Daily Backup of VM at 3:00 AM using Vault and Retain an Old Backup

### Resources
- [YouTube Video](https://www.youtube.com/watch?v=A0jAeGf2zUQ)
- [Microsoft Learn](https://learn.microsoft.com/en-us/training/paths/azure-administrator-monitor-backup-resources/)
- [YouTube Video](https://www.youtube.com/watch?v=DQywse_j8l8)
- [Microsoft Learn](https://learn.microsoft.com/en-us/training/paths/azure-administrator-monitor-backup-resources/)

### Steps
1. **Create a Recovery Services Vault**:
    - Sign in to the [Azure portal](https://portal.azure.com/)
    - Create a resource and search for "Backup and Site Recovery (OMS)".
    - Configure the vault with a unique name, subscription, resource group, and location.
    - Review and create the vault.

2. **Configure Backup for the VM**:
    - Navigate to the Recovery Services vault.
    - Click on Backup under Getting Started.
    - Set workload running in Azure and backup for Virtual machine.

3. **Create a Backup Policy**:
    - Create a new backup policy.
    - Set the policy name, backup frequency to daily at 3:00 AM, and retention range to 30 days.

4. **Apply the Backup Policy to the VM**:
    - Select the VM(s) to back up.
    - Click Enable Backup.

5. **Verify Backup Configuration**:
    - Go to Protected Items under the Recovery Services vault.
    - Ensure the VM is listed with the applied backup policy.

6. **Configure Retention**:
    - Navigate to the Backup Policies section in the Recovery Services vault.
    - Edit the backup policy created earlier.
    - Set the retention range to retain the backup taken every day at 3:00 AM for 30 days.

## Conclusion

By following the detailed steps in this guide, you can complete the tasks required for managing Azure infrastructure, including scheduling VM backups, creating alert rules, and provisioning backups in the backup center. For further assistance, refer to the provided resources or contact Azure support.
