To create new project, make sure *charyf* gem is installed and executable is working by typing ```charyf``` into your terminal.

Generating new project is very easy if you are familiar with the [*rails*](https://github.com/rails/rails) framework, as *charyf* uses [*thor*](https://github.com/erikhuda/thor) for building command line tools as well.

To generate new project run ``charyf new example_bot`` in your terminal.  
This will create directory called *example_bot* with application *ExampleBot*.  
Running said command will also initialize git repository: use ``-G`` or ``--skip-git`` to skip this feature.

Using ``-lib`` options, ``-skip-git`` option will be forced. When installing charyf as library, all files will be nested into directory named **charyf** insite the app directory. This is meant to prevent collisions with similar file structures such as ruby on rails.

You can configure your charyf application during generation phase by setting enabled intent processors and storage providers. See [[Configuration]] to learn more. Available strategies are always listed in command help. ``charyf -h``

