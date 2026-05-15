# OpenSOC

OpenSOC is a documented SOC lab series. The repo currently tracks only what has been covered in the published posts:

- [OpenSOC: Building an Open Source SOC Lab That Does Not Suck](https://iamb4uc.xyz/post/opensoc-intro/)
- [OpenSOC: Setting up the SIEM (Wazuh Server)](https://iamb4uc.xyz/post/opensoc-wazuh-setup/)

The point of this repo is to keep a clean paper trail for the lab as it is built. It should not contain placeholder directories, fake runbooks, or documentation for components that have not been covered yet.

## What Is Covered

The current docs cover:

- Why OpenSOC exists.
- The basic SOC loop: collect, detect, alert, preserve evidence, review, and improve.
- The initial lab direction.
- Wazuh as the first SIEM.
- Wazuh server installation with the official quickstart script.
- Dashboard login and password recovery notes.

## Documentation

- [Docs index](docs/README.md)
- [OpenSOC intro](docs/opensoc-intro.md)
- [Wazuh server setup](docs/wazuh-installation.md)

## Not Covered Yet

The intro post mentions future work such as agents, `auditd`, `osquery`, FleetDM OSS, Suricata, Zeek, SOAR, Windows/macOS agents, and Splunk. Those are not documented here yet because the published setup posts have not covered them. I will implement them and get them documented here along with config files and other stuffs

## License

OpenSOC is released under the GNU General Public License v3.0. See [LICENSE](LICENSE).
