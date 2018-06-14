All sample config are from https://logging.apache.org/log4net/release/config-examples.html

In order to load automatically the configuration it is possible to add the following line to the assembly.cs

[assembly: log4net.Config.XmlConfigurator(Watch=true)] 


SQL Query to create the log table

CREATE TABLE [dbo].[Log] (
    [Id] [int] IDENTITY (1, 1) NOT NULL,
    [Date] [datetime] NOT NULL,
    [Thread] [varchar] (255) NOT NULL,
    [Level] [varchar] (50) NOT NULL,
    [Logger] [varchar] (255) NOT NULL,
    [Message] [varchar] (4000) NOT NULL,
    [Exception] [varchar] (2000) NULL
)