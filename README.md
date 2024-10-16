# How to Start Odoo Project

### Clone the gitrepo

```
https://github.com/eshafik/odoo-boilerplate.git
```

### The functions of the subdirectories are as follows:

 - src/: This contains the clone of Odoo itself, as well as various third-party add-on projects.
 - local/: This is used to save your instance-specific add-ons
 - bin/: This includes various helper executable shell scripts
 - filestore/: This is used as a file store
 - logs/ (optional): This is used to store the server log files

### Clone your odoo version to the src directory

```
git clone -b 17.0 --single-branch --depth 1 https://github.
com/odoo/odoo.git src/odoo
```

### In the src directory you can also clone any thirdparty addons directory also.

### Create virtual environment in the parent directory and install dependency

```
python3 -m venv venv
source venv/bin/activate
pip install -r src/odoo/requirements.txt
```

### Make the bin/odoo file executable:

```
chmod +x bin/odoo
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
