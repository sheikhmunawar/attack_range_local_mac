## [For MacOS](https://github.com/splunk/attack_range_local/wiki/MacOS-Installation)

#### Clone the git repo
```
git clone git@github.com:sheikhmunawar/attack_range_local_mac.git
```

#### Prerequisite:
```
vmi ~/.zshrc
export PATH="$PATH:/Users/mac/Library/Python/3.8/bin"

python3 --version

python3 -m venv .venv		## change python version available in local system
source .venv/bin/activate

python --version
pip --version
pip install --upgrade pip
pip --version

pip install ansible
pip install ansible-runner
pip install python-vagrant
pip install pywinrm
pip install splunk-sdk
pip install tabulate
ansible-galaxy collection install community.windows

```

## Vagrant configuration
```
brew install --cask virtualbox if you don't already have virtual box installed on OSX, otherwise see their installation instructions.
brew install --cask vagrant install Vagrant CLI on OSX, otherwise see: guide
Change splunk_admin_password and win_password in attack_range_local.conf
```

## Download Assets
```
cd /Users/mac/Workspace/Splunk/downloads

wget -i appDownloadLinks.txt
wget -nc -i appDownloadLinks.txt

https://download.splunk.com/products/splunk/releases/8.0.2/linux/splunk-8.0.2-a7f645ddaf91-Linux-x86_64.tgz
https://attack-range-appbinaries.s3-us-west-2.amazonaws.com
https://attack-range-appbinaries.s3-us-west-2.amazonaws.com/splunk-add-on-for-microsoft-windows_800.tgz
https://attack-range-appbinaries.s3-us-west-2.amazonaws.com/splunk-add-on-for-microsoft-sysmon_1062.tgz

https://attack-range-appbinaries.s3-us-west-2.amazonaws.com/splunk-common-information-model-cim_4180.tgz
https://attack-range-appbinaries.s3-us-west-2.amazonaws.com/DA-ESS-ContentUpdate-latest.tar.gz
https://attack-range-appbinaries.s3-us-west-2.amazonaws.com/Splunk_ASX-latest.tar.gz
https://attack-range-appbinaries.s3-us-west-2.amazonaws.com/python-for-scientific-computing-for-linux-64-bit_200.tgz
https://attack-range-appbinaries.s3-us-west-2.amazonaws.com/splunk-machine-learning-toolkit_510.tgz
https://attack-range-appbinaries.s3-us-west-2.amazonaws.com/splunk-stream_720.tgz
https://attack-range-appbinaries.s3-us-west-2.amazonaws.com/splunk-security-essentials_310.tgz
https://attack-range-appbinaries.s3-us-west-2.amazonaws.com/punchcard-custom-visualization_140.tgz
https://attack-range-appbinaries.s3-us-west-2.amazonaws.com/status-indicator-custom-visualization_140.tgz
https://attack-range-appbinaries.s3-us-west-2.amazonaws.com/splunk_attack_range_reporting-1.0.5.tar.gz
https://attack-range-appbinaries.s3-us-west-2.amazonaws.com/timeline-custom-visualization_140.tgz
https://attack-range-appbinaries.s3-us-west-2.amazonaws.com/splunk-add-on-for-amazon-web-services_500.tgz
https://attack-range-appbinaries.s3-us-west-2.amazonaws.com/phantom-app-for-splunk_305.tgz
https://download.splunk.com/products/universalforwarder/releases/8.0.2/windows/splunkforwarder-8.0.2-a7f645ddaf91-x64-release.msi
https://attack-range-appbinaries.s3-us-west-2.amazonaws.com/Sysmon.zip
https://attack-range-appbinaries.s3-us-west-2.amazonaws.com/splunk-add-on-for-microsoft-sysmon_1062.tgz
https://attack-range-appbinaries.s3-us-west-2.amazonaws.com/splunk-machine-learning-toolkit_510.tgz
https://dl.google.com/go/go1.13.11.linux-amd64.tar.gz

https://s3.amazonaws.com/botsdataset/botsv1/splunk-pre-indexed/botsv1_data_set.tgz
https://s3.amazonaws.com/botsdataset/botsv1/botsv1-attack-only.tgz
https://s3.amazonaws.com/botsdataset/botsv2/botsv2_data_set.tgz
https://s3.amazonaws.com/botsdataset/botsv2/botsv2_data_set_attack_only.tgz
https://botsdataset.s3.amazonaws.com/botsv3/botsv3_data_set.tgz
```
