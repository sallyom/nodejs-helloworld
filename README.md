Nodejs app created from OpenShift 2.2 cartridge migrated to OpenShift 3.x
-------------------------------------------------------------------------

**Modifications from v2 -> v3**

* Removed .openshift dir
* L107: Replaced 'self.app = express.createServer();' in server.js with 'self.app = express();'
* L25: self.ipaddress = process.env.IP   || process.env.OPENSHIFT_NODEJS_IP || '0.0.0.0';
* L26: self.port      = process.env.PORT || process.env.OPENSHIFT_NODEJS_PORT || 8080;
