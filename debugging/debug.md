
cf enable-ssh <service_name>
example:
cf enable-ssh incident-management-srv
cf restart incident-management-srv


cf ssh incident-management-srv

ps aux | grep "node" (get PID)
kill -usr1 <PID>

## Enable port forwarding
cf ssh -N -L 9229:127.0.0.1:9229 incident-management-srv