# Wazuh Server Setup

Source post: https://iamb4uc.xyz/post/opensoc-wazuh-setup/

This is the first actual setup step in the OpenSOC series: installing the Wazuh server as the initial SIEM.

Wazuh is used here because it is open source, free to use, and quick to get running for a lab.

## Requirements

Use a Debian or Ubuntu server installation.

Minimum VM or machine size from the post:

- CPU: 8 cores
- RAM: 8 GB or higher
- Disk: 100 GB or higher

## Install Wazuh

On the Wazuh server, run the quickstart installer:

```sh
curl -sO https://packages.wazuh.com/4.14/wazuh-install.sh && sudo bash ./wazuh-install.sh -a
```

The installer sets up Wazuh and prints the credentials needed for the dashboard.

## Log In

Open the Wazuh server in a browser with HTTPS:

```text
https://<WAZUH_SERVER_IP>
```

Use:

```text
username: admin
password: <password from installer output>
```

If a Chromium-based browser has issues, try Firefox. Also make sure you are using `https`, not `http`.

## Recover The Admin Password

The installer also stores credentials in the tar file created during installation.

Run:

```sh
sudo tar -axf wazuh-install-files.tar wazuh-install-files/wazuh-password.txt -O | grep -P "\'admin\'" -A 1
```

Use the recovered password to log in as `admin`.

## Next Step

The next blog will cover agents. Agent setup is not documented in this repo yet.
