# silk templates
### templates for the Silk Web Toolkit

Components can be used to give look and feel to sections of, or entire websites/webapps.  Templates wrap around views.
Build whatever templates you need, complement the limited core templates bundled with Silk.

## how to build a template
### manually

* have a look at the handful of samples under org/silkyweb
* find or create a package directory to place your template in
  * placing templates in packages helps guarantee uniqueness
* name your template something sensible
  * 'template-missing' will be used by Silk if your template can not be found
* create a directory with the same name as the version of Silk you are using
  * just use the major.minor.patch ie 0.1.0
* create the required .dna config directory
* add a dna.conf definition to .dna, see the examples under org/silkyweb
  * check your package value is the same as the directory hierarchy you have placed your template in
  * silk-version is the version of Silk the template has been built and tested against
  * it is useful to add a quick description of the purpose of the template
* add the template see the examples under /org/silkyweb
  * ensure the filename is the same as the template's name
  * ensure it has an id along the lines of silk-template
* test your template by including it in a silk site and 'spinning'

### or with silk

* 'silk template-clone some-template'
* modify the .dna/dna.conf file to suit
* rename and modify the template file to suit 
* in your template's parent directory 'silk template-install'


## how to contribute

### you

* fork this repository
* add your component
* submit a pull request

### us

* review your pull request
* add to silk template repository so your template is available with 'silk update'
