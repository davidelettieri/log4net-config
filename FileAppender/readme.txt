All sample config are from https://logging.apache.org/log4net/release/config-examples.html

In order to load automatically the configuration it is possible to add the following line to the assembly.cs

[assembly: log4net.Config.XmlConfigurator(Watch=true)] 