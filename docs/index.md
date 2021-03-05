---
layout: default
---
# Nebula Logger: Documentation
# Classes
## logger-engine

### [FlowLogEntry](docs/logger-engine/FlowLogEntry.md)


Handles adding new log entries in Flow



### [FlowRecordLogEntry](docs/logger-engine/FlowRecordLogEntry.md)


Handles adding new log entries in Flow for a particular SObject record



### [LogEntryEventBuilder](docs/logger-engine/LogEntryEventBuilder.md)


Builder class that generates each LogEntryEvent__c record



### [LogMessage](docs/logger-engine/LogMessage.md)


Provides the ability to generate string messages on demand, using String.format()



### [Logger](docs/logger-engine/Logger.md)


The core class for logging


## log-management

### [LogBatchPurgeScheduler](docs/log-management/LogBatchPurgeScheduler.md)


Schedulable class used to schedule the batch job LogBatchPurger



### [LogBatchPurger](docs/log-management/LogBatchPurger.md)


Batch class used to delete old logs, based on Log__c.LogRetentionDate__c <= :System.today()



### [LogEntryEventHandler](docs/log-management/LogEntryEventHandler.md)


Subscribes to LogEntryEvent__e platform events and normalizes the data into Log__c and LogEntry__c records



### [LogEntryFieldSetPicklist](docs/log-management/LogEntryFieldSetPicklist.md)


Dynamically returns LogEntry__c field sets in App Builder when configuring the component RelatedLogEntries



### [LogEntryHandler](docs/log-management/LogEntryHandler.md)


Manages setting fields on LogEntry__c before insert & update



### [LogHandler](docs/log-management/LogHandler.md)


Manages setting fields on Log__c before insert & update



### [RelatedLogEntriesController](docs/log-management/RelatedLogEntriesController.md)


Controller class for the component RelatedLogEntries


## packaging

### [LoggerInstallHandler](docs/packaging/LoggerInstallHandler.md)


Automatically enables org default settings when installing the managed package


