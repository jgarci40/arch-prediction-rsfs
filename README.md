# Architecture Mappings for Architectural Decay Prediction

This README file describes the recovered architectural mappings used for architectural decay prediction. 

## Directory Structure

The recovered architectural mappings are structured as follows:

```
RSFFiles
├── [Project Name]
│   ├── ARC modules
│   │   ├── [Project Name]-[Version Info]
│   │   │   └── ARC.rsf
│   └── Package\modules
│       ├── [Project Name]-[Version Info]-src_pkgs.rsf
```

For example, consider the Apache Camel project:

```
.
├── Camel
│   ├── ARC modules
│   │   ├── apache-camel-1.6.0
│   │   │   └── ARC.rsf
│   │   ├── apache-camel-2.0-M3-2009-07-26
│   │   │   └── ARC.rsf
│   │   ├── apache-camel-2.2.0-2010-02-16
│   │   │   └── ARC.rsf
│   │   ├── apache-camel-2.4.0-2010-07-16
│   │   │   └── ARC.rsf
│   │   ├── apache-camel-2.5.0-2010-10-31
│   │   │   └── ARC.rsf
│   │   ├── apache-camel-2.6.0-2011-01-29
│   │   │   └── ARC.rsf
│   │   ├── apache-camel-2.7.1-2011-04-13
│   │   │   └── ARC.rsf
│   │   ├── apache-camel-2.8.0-2011-07-25
│   │   │   └── ARC.rsf
│   │   └── apache-camel-2.8.3-2011-11-22
│   │       └── ARC.rsf
│   └── Package modules
│       ├── apache-camel-1.6.0-src_pkgs.rsf
│       ├── apache-camel-2.0-M3-src_pkgs.rsf
│       ├── apache-camel-2.2.0-src_pkgs.rsf
│       ├── apache-camel-2.4.0-src_pkgs.rsf
│       ├── apache-camel-2.5.0-src_pkgs.rsf
│       ├── apache-camel-2.6.0-src_pkgs.rsf
│       ├── apache-camel-2.7.1-src_pkgs.rsf
│       ├── apache-camel-2.8.0-src_pkgs.rsf
│       └── apache-camel-2.8.3-src_pkgs.rsf
```

The above example for Apache Camel contains 18 recovered architectures, nine for ARC and another nine for packages.

## The Format of Recovered Architecture Files

The recovered architecture files are in the Rigi Standard Format (RSF), where each line in the file is a triple of the following form:
```contain [module ID m] [entity name e]```. This format means that the entity *e* has been mapped to, or belongs to, module *m*.

For example, consider the following line: ```contain 0 org.apache.camel.component.bean.CamelInvocationHandler```. This line indicates that org.apache.camel.component.bean.CamelInvocationHandler belongs to module 0. 