---
layout: default
---

# Apex Documentation

# Classes

## logger-engine

### [FlowLogEntry](NebulaLogger/logger-engine/FlowLogEntry)

Handles adding new log entries in Flow

### [FlowRecordLogEntry](NebulaLogger/logger-engine/FlowRecordLogEntry)

Handles adding new log entries in Flow for a particular `SObject` record

### [LogEntryEventBuilder](NebulaLogger/logger-engine/LogEntryEventBuilder)

Builder class that generates each `LogEntryEvent__c` record

### [LogMessage](NebulaLogger/logger-engine/LogMessage)

Provides the ability to generate string messages on demand, using String.format()

### [Logger](NebulaLogger/logger-engine/Logger)

The core class for logging

## log-management

### [LogBatchPurgeScheduler](NebulaLogger/log-management/LogBatchPurgeScheduler)

Schedulable class used to schedule the batch job `LogBatchPurger`

### [LogBatchPurger](NebulaLogger/log-management/LogBatchPurger)

Batch class used to delete old logs, based on `Log__c.LogRetentionDate__c <= :System.today()`

### [LogEntryEventHandler](NebulaLogger/log-management/LogEntryEventHandler)

Subscribes to `LogEntryEvent__e` platform events and normalizes the data into `Log__c` and `LogEntry__c` records

### [LogEntryFieldSetPicklist](NebulaLogger/log-management/LogEntryFieldSetPicklist)

Dynamically returns `LogEntry__c` field sets in App Builder when configuring the component RelatedLogEntries

### [LogEntryHandler](NebulaLogger/log-management/LogEntryHandler)

Manages setting fields on `LogEntry__c` before insert & before update

### [LogHandler](NebulaLogger/log-management/LogHandler)

Manages setting fields on `Log__c` before insert & before update

### [RelatedLogEntriesController](NebulaLogger/log-management/RelatedLogEntriesController)

Controller class for the component RelatedLogEntries

## packaging

### [LoggerInstallHandler](NebulaLogger/packaging/LoggerInstallHandler)

Automatically enables org default settings when installing the managed package
