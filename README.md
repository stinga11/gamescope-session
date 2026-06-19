Enable passwordless restarts; required for non-TTY execution.
sudo visudo -f /etc/sudoers.d/plasmalogin-restart
deck ALL=(ALL) NOPASSWD: /usr/bin/systemctl restart plasmalogin.service
