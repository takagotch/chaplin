### chaplin
---
https://github.com/chaplinjs/chaplin

```coffee
// test/sync_machine_spec.coffee
Backbone = require 'backbone'
sinon = require 'sinon'
{SyncMachine} = require '../src/chapin'

describe 'SyncMachine', ->
  machine = null
  
  beforeEach ->
    machine = {}
    Object.assign machine, Backbone.Events
    Object.assign machine, SyncMachine
  
  it 'should change its state', ->
    expect(machine.syncState()).to.equal 'unsynced'
    
    machine.beginSync()
    expect(machine.syncState()).to.equal 'syncing'

```

```
```

```
```

