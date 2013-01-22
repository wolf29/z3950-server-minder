z3950-server-minder
===================

Another minder script to watch, in this case, 
an Evergreen-ILS z3950 server
This is a small script to check if there is a running 
instance of simple2zoom.pm.  If not, the script automatically 
starts simple2zoom.  This particular version of the script runs 
on the http://evergreen.lyrasistechnology.org server on port 210
The z3950 server there is just to take stress off of other servers 
where there are actually some bibs, authorities and holdings.


simple2zoom -c /openils/conf/oils_z3950.xml -- -f \
/openils/conf/xml2marc-yaz.cfg <your-z3950-server:210 &


