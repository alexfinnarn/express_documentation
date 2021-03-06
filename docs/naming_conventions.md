## What to Name a Module, Feature or Bundle?

Naming code is often referenced as one of the 2 truly difficult parts of coding ([along with caching invalidation and off by one errors](https://twitter.com/codinghorror/status/506010907021828096)). Naming in Express is no exception. While we haven't always followed this pattern, this is the current recommendation.

To be recognized by Profile Module Manager, a module name must end in _bundle. The bundles prefix should indicate it's intended use.

**express_** Any bundle or module that is not CU specific, but is being designed to work within Express.  Examples are express_layout, express_permissions, etc

**cu_** Express specific code that is unlikely to have much value beyond a reference to another group. In D7 this was used for all code writen for CU Boulder.  In D8, the cu_ underscore will indicate that it has been designed to work with any organization within the CU system.

**ucb_** this was not used in D7.  In D8, this will indicate that the code is specific to CU Boulder. D7 modules like cu_ldap and cu_altas will use ucb_ in D8 since they are specific to the Boulder campus.

**custom_** for a site specific bundle that is unlikely to be used on more than one site

Modules that are not specific to CU or Express that may be useful as contrib should be named accordingly.  User [External Invite](https://www.drupal.org/project/user_external_invite) and [Profile Module Manager](https://www.drupal.org/project/profile_module_manager) are good examples of this.
