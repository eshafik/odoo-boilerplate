# How to Start Odoo Project

### Clone the gitrepo

```
https://github.com/eshafik/odoo-boilerplate.git
```

### Now save initial configuration to the config file. Run-

```
bin/odoo --stop-after-init --save \
--addons-path src/odoo/odoo/addons,src/odoo/addons,local \
--data-dir filestore
```

It will create odoo-boilerplate.cfg file.

### Now modify the odoo-boilerplate.cfg with the database credentials

# That's it!!!

If you need to upgrade the odoo version just go to the _src/odoo_ and now you can switch your version.
