1️⃣ ps aux | grep ssh

Observation:

Verified ssh process is running

Understood how to identify PID

Realized how useful grep filtering is

2️⃣ systemctl status ssh

Observation:

Shows service state (active/running)

Displays recent logs

Good for quick health check

3️⃣ journalctl -u ssh -n 10

Observation:

Shows last 10 logs

Helpful for debugging failed restarts
===========================
top → check CPU/memory usage

df -h → check disk space

free -m → check RAM usage

systemctl status <service> → check service health

journalctl -xe → check detailed errors

These give quick system overview during production issue.

=================
1️⃣ Which 3 commands save you most time right now?

systemctl status → Instant service visibility

df -h → Quick disk troubleshooting

ls -l → Understand permissions immediately
