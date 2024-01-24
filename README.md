This is the Test ACE Messageflow with the issues when using node-for-log4j v2.0.2 in ACE V11.0.0.24 on Windows.

The issues are described (and fixed) here:

+ https://github.com/ot4i/node-for-log4j/issues/9
+ https://github.com/ot4i/node-for-log4j/issues/10

Thanks to the author for the fast support and fix.

Basically, we need to do one of the two options below to fix the issues:

+ Set Log4jConfigFile = brokerlog.xml in the node and put the file brokerlog.xml in the classes directory of the installation (C:\Program Files\IBM\ACE\11.0.0.24\server\classes)

+ Set Log4jConfigFile = /C:/temp/brokerlog.xml in the node (configure the path with leading "/") and put the file brokerlog.xml to C:/temp/


