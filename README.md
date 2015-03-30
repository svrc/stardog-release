# stardog-release
BOSH release for http://stardog.com

Work in progress; doesn't work yet.   You can create a BOSH release and upload it but the deploy won't work quite yet.

This is a modification of the Zookeeper BOSH release (open source), extra bits from that that are 
unnecessary with stardog still need to be removed.

Bugs:
# properites.sh -- get rid of it
# BOSH persistent disk /var/vcap/store should be used for $STARDOG_HOME on stardog-node jobs
# log4j.proeprties filename typo
# Zookeeper PIDFILE is in wrong location, currently export PIDFILE=/var/vcap/store/zookeeper/zookeeper_server.pid
# slf4j package in stardog-node should be configured to use log4j
# Remove "stardog-3.0" from STARDOG_INSTALL=${JOB_DIR}/packages/stardog/stardog-3.0"


