## 🔧 Configuration: Passwordless Restart

Enable passwordless restarts; required for non-TTY execution.

Run the following command to create and edit the specific configuration file:

```bash
sudo visudo -f /etc/sudoers.d/plasmalogin-restart
```

Add this line inside the file to grant the necessary permissions:

```
deck ALL=(ALL) NOPASSWD: /usr/bin/systemctl restart plasmalogin.service
```
