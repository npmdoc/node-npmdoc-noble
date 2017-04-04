# api documentation for  [noble (v1.8.0)](https://github.com/sandeepmistry/noble)  [![npm package](https://img.shields.io/npm/v/npmdoc-noble.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-noble) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-noble.svg)](https://travis-ci.org/npmdoc/node-npmdoc-noble)
#### A Node.js BLE (Bluetooth Low Energy) central library.

[![NPM](https://nodei.co/npm/noble.png?downloads=true)](https://www.npmjs.com/package/noble)

[![apidoc](https://npmdoc.github.io/node-npmdoc-noble/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-noble_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-noble/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-noble/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-noble/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Sandeep Mistry",
        "email": "sandeep.mistry@gmail.com"
    },
    "browser": {
        "./lib/resolve-bindings.js": "./lib/resolve-bindings-web.js"
    },
    "bugs": {
        "url": "https://github.com/sandeepmistry/noble/issues"
    },
    "dependencies": {
        "bluetooth-hci-socket": "^0.5.1",
        "bplist-parser": "0.0.6",
        "debug": "~2.2.0",
        "xpc-connection": "~0.1.4"
    },
    "description": "A Node.js BLE (Bluetooth Low Energy) central library.",
    "devDependencies": {
        "async": "~0.2.9",
        "jshint": "latest",
        "mocha": "~1.8.2",
        "should": "~1.2.2",
        "sinon": "~1.6.0",
        "ws": "~0.4.31"
    },
    "directories": {},
    "dist": {
        "shasum": "6fea67f6f6b46dd9704e29549603a1b3c56d305b",
        "tarball": "https://registry.npmjs.org/noble/-/noble-1.8.0.tgz"
    },
    "engines": {
        "node": ">=0.8"
    },
    "gitHead": "18c51f0feed477849dbb3d9c58f19dddfe32632a",
    "homepage": "https://github.com/sandeepmistry/noble",
    "keywords": [
        "bluetooth",
        "BLE",
        "bluetooth low energy",
        "bluetooth smart",
        "central"
    ],
    "license": "MIT",
    "main": "./index.js",
    "maintainers": [
        {
            "name": "sandeepmistry",
            "email": "sandeep.mistry@gmail.com"
        }
    ],
    "name": "noble",
    "optionalDependencies": {
        "bluetooth-hci-socket": "^0.5.1",
        "bplist-parser": "0.0.6",
        "xpc-connection": "~0.1.4"
    },
    "os": [
        "darwin",
        "linux",
        "freebsd",
        "win32"
    ],
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/sandeepmistry/noble.git"
    },
    "scripts": {
        "pretest": "jshint *.js lib/. test/.",
        "test": "mocha -R spec test/*.js"
    },
    "version": "1.8.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module noble](#apidoc.module.noble)
1.  [function <span class="apidocSignatureSpan"></span>noble (bindings)](#apidoc.element.noble.noble)
1.  [function <span class="apidocSignatureSpan">noble.</span>characteristic (noble, peripheralId, serviceUuid, uuid, properties)](#apidoc.element.noble.characteristic)
1.  [function <span class="apidocSignatureSpan">noble.</span>descriptor (noble, peripheralId, serviceUuid, characteristicUuid, uuid)](#apidoc.element.noble.descriptor)
1.  [function <span class="apidocSignatureSpan">noble.</span>peripheral (noble, id, address, addressType, connectable, advertisement, rssi)](#apidoc.element.noble.peripheral)
1.  [function <span class="apidocSignatureSpan">noble.</span>service (noble, peripheralId, uuid)](#apidoc.element.noble.service)
1.  number <span class="apidocSignatureSpan">noble.</span>_eventsCount
1.  object <span class="apidocSignatureSpan">noble.</span>_bindings
1.  object <span class="apidocSignatureSpan">noble.</span>_bindings._events
1.  object <span class="apidocSignatureSpan">noble.</span>_characteristics
1.  object <span class="apidocSignatureSpan">noble.</span>_descriptors
1.  object <span class="apidocSignatureSpan">noble.</span>_discoveredPeripheralUUids
1.  object <span class="apidocSignatureSpan">noble.</span>_events
1.  object <span class="apidocSignatureSpan">noble.</span>_peripherals
1.  object <span class="apidocSignatureSpan">noble.</span>_services
1.  object <span class="apidocSignatureSpan">noble.</span>characteristic.prototype
1.  object <span class="apidocSignatureSpan">noble.</span>descriptor.prototype
1.  object <span class="apidocSignatureSpan">noble.</span>noble.prototype
1.  object <span class="apidocSignatureSpan">noble.</span>peripheral.prototype
1.  object <span class="apidocSignatureSpan">noble.</span>service.prototype
1.  string <span class="apidocSignatureSpan">noble.</span>address
1.  string <span class="apidocSignatureSpan">noble.</span>state

#### [module noble._bindings](#apidoc.module.noble._bindings)
1.  [function <span class="apidocSignatureSpan">noble._bindings.</span>onSigIntBinded ()](#apidoc.element.noble._bindings.onSigIntBinded)
1.  number <span class="apidocSignatureSpan">noble._bindings.</span>_eventsCount
1.  object <span class="apidocSignatureSpan">noble._bindings.</span>_aclStreams
1.  object <span class="apidocSignatureSpan">noble._bindings.</span>_addresseTypes
1.  object <span class="apidocSignatureSpan">noble._bindings.</span>_addresses
1.  object <span class="apidocSignatureSpan">noble._bindings.</span>_connectable
1.  object <span class="apidocSignatureSpan">noble._bindings.</span>_connectionQueue
1.  object <span class="apidocSignatureSpan">noble._bindings.</span>_events
1.  object <span class="apidocSignatureSpan">noble._bindings.</span>_gap
1.  object <span class="apidocSignatureSpan">noble._bindings.</span>_gatts
1.  object <span class="apidocSignatureSpan">noble._bindings.</span>_handles
1.  object <span class="apidocSignatureSpan">noble._bindings.</span>_hci
1.  object <span class="apidocSignatureSpan">noble._bindings.</span>_pendingConnectionUuid
1.  object <span class="apidocSignatureSpan">noble._bindings.</span>_signalings
1.  string <span class="apidocSignatureSpan">noble._bindings.</span>_state

#### [module noble._bindings._events](#apidoc.module.noble._bindings._events)
1.  [function <span class="apidocSignatureSpan">noble._bindings._events.</span>addressChange ()](#apidoc.element.noble._bindings._events.addressChange)
1.  [function <span class="apidocSignatureSpan">noble._bindings._events.</span>broadcast ()](#apidoc.element.noble._bindings._events.broadcast)
1.  [function <span class="apidocSignatureSpan">noble._bindings._events.</span>characteristicsDiscover ()](#apidoc.element.noble._bindings._events.characteristicsDiscover)
1.  [function <span class="apidocSignatureSpan">noble._bindings._events.</span>connect ()](#apidoc.element.noble._bindings._events.connect)
1.  [function <span class="apidocSignatureSpan">noble._bindings._events.</span>descriptorsDiscover ()](#apidoc.element.noble._bindings._events.descriptorsDiscover)
1.  [function <span class="apidocSignatureSpan">noble._bindings._events.</span>disconnect ()](#apidoc.element.noble._bindings._events.disconnect)
1.  [function <span class="apidocSignatureSpan">noble._bindings._events.</span>discover ()](#apidoc.element.noble._bindings._events.discover)
1.  [function <span class="apidocSignatureSpan">noble._bindings._events.</span>handleNotify ()](#apidoc.element.noble._bindings._events.handleNotify)
1.  [function <span class="apidocSignatureSpan">noble._bindings._events.</span>handleRead ()](#apidoc.element.noble._bindings._events.handleRead)
1.  [function <span class="apidocSignatureSpan">noble._bindings._events.</span>handleWrite ()](#apidoc.element.noble._bindings._events.handleWrite)
1.  [function <span class="apidocSignatureSpan">noble._bindings._events.</span>includedServicesDiscover ()](#apidoc.element.noble._bindings._events.includedServicesDiscover)
1.  [function <span class="apidocSignatureSpan">noble._bindings._events.</span>notify ()](#apidoc.element.noble._bindings._events.notify)
1.  [function <span class="apidocSignatureSpan">noble._bindings._events.</span>read ()](#apidoc.element.noble._bindings._events.read)
1.  [function <span class="apidocSignatureSpan">noble._bindings._events.</span>rssiUpdate ()](#apidoc.element.noble._bindings._events.rssiUpdate)
1.  [function <span class="apidocSignatureSpan">noble._bindings._events.</span>scanStart ()](#apidoc.element.noble._bindings._events.scanStart)
1.  [function <span class="apidocSignatureSpan">noble._bindings._events.</span>scanStop ()](#apidoc.element.noble._bindings._events.scanStop)
1.  [function <span class="apidocSignatureSpan">noble._bindings._events.</span>servicesDiscover ()](#apidoc.element.noble._bindings._events.servicesDiscover)
1.  [function <span class="apidocSignatureSpan">noble._bindings._events.</span>stateChange ()](#apidoc.element.noble._bindings._events.stateChange)
1.  [function <span class="apidocSignatureSpan">noble._bindings._events.</span>valueRead ()](#apidoc.element.noble._bindings._events.valueRead)
1.  [function <span class="apidocSignatureSpan">noble._bindings._events.</span>valueWrite ()](#apidoc.element.noble._bindings._events.valueWrite)
1.  [function <span class="apidocSignatureSpan">noble._bindings._events.</span>write ()](#apidoc.element.noble._bindings._events.write)

#### [module noble._events](#apidoc.module.noble._events)
1.  [function <span class="apidocSignatureSpan">noble._events.</span>warning ()](#apidoc.element.noble._events.warning)

#### [module noble.characteristic](#apidoc.module.noble.characteristic)
1.  [function <span class="apidocSignatureSpan">noble.</span>characteristic (noble, peripheralId, serviceUuid, uuid, properties)](#apidoc.element.noble.characteristic.characteristic)
1.  [function <span class="apidocSignatureSpan">noble.characteristic.</span>super_ ()](#apidoc.element.noble.characteristic.super_)

#### [module noble.characteristic.prototype](#apidoc.module.noble.characteristic.prototype)
1.  [function <span class="apidocSignatureSpan">noble.characteristic.prototype.</span>broadcast (broadcast, callback)](#apidoc.element.noble.characteristic.prototype.broadcast)
1.  [function <span class="apidocSignatureSpan">noble.characteristic.prototype.</span>discoverDescriptors (callback)](#apidoc.element.noble.characteristic.prototype.discoverDescriptors)
1.  [function <span class="apidocSignatureSpan">noble.characteristic.prototype.</span>notify (notify, callback)](#apidoc.element.noble.characteristic.prototype.notify)
1.  [function <span class="apidocSignatureSpan">noble.characteristic.prototype.</span>read (callback)](#apidoc.element.noble.characteristic.prototype.read)
1.  [function <span class="apidocSignatureSpan">noble.characteristic.prototype.</span>subscribe (callback)](#apidoc.element.noble.characteristic.prototype.subscribe)
1.  [function <span class="apidocSignatureSpan">noble.characteristic.prototype.</span>toString ()](#apidoc.element.noble.characteristic.prototype.toString)
1.  [function <span class="apidocSignatureSpan">noble.characteristic.prototype.</span>unsubscribe (callback)](#apidoc.element.noble.characteristic.prototype.unsubscribe)
1.  [function <span class="apidocSignatureSpan">noble.characteristic.prototype.</span>write (data, withoutResponse, callback)](#apidoc.element.noble.characteristic.prototype.write)

#### [module noble.descriptor](#apidoc.module.noble.descriptor)
1.  [function <span class="apidocSignatureSpan">noble.</span>descriptor (noble, peripheralId, serviceUuid, characteristicUuid, uuid)](#apidoc.element.noble.descriptor.descriptor)
1.  [function <span class="apidocSignatureSpan">noble.descriptor.</span>super_ ()](#apidoc.element.noble.descriptor.super_)

#### [module noble.descriptor.prototype](#apidoc.module.noble.descriptor.prototype)
1.  [function <span class="apidocSignatureSpan">noble.descriptor.prototype.</span>readValue (callback)](#apidoc.element.noble.descriptor.prototype.readValue)
1.  [function <span class="apidocSignatureSpan">noble.descriptor.prototype.</span>toString ()](#apidoc.element.noble.descriptor.prototype.toString)
1.  [function <span class="apidocSignatureSpan">noble.descriptor.prototype.</span>writeValue (data, callback)](#apidoc.element.noble.descriptor.prototype.writeValue)

#### [module noble.noble](#apidoc.module.noble.noble)
1.  [function <span class="apidocSignatureSpan">noble.</span>noble (bindings)](#apidoc.element.noble.noble.noble)
1.  [function <span class="apidocSignatureSpan">noble.noble.</span>super_ ()](#apidoc.element.noble.noble.super_)

#### [module noble.noble.prototype](#apidoc.module.noble.noble.prototype)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>broadcast (peripheralUuid, serviceUuid, characteristicUuid, broadcast)](#apidoc.element.noble.noble.prototype.broadcast)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>connect (peripheralUuid)](#apidoc.element.noble.noble.prototype.connect)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>disconnect (peripheralUuid)](#apidoc.element.noble.noble.prototype.disconnect)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>discoverCharacteristics (peripheralUuid, serviceUuid, characteristicUuids)](#apidoc.element.noble.noble.prototype.discoverCharacteristics)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>discoverDescriptors (peripheralUuid, serviceUuid, characteristicUuid)](#apidoc.element.noble.noble.prototype.discoverDescriptors)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>discoverIncludedServices (peripheralUuid, serviceUuid, serviceUuids)](#apidoc.element.noble.noble.prototype.discoverIncludedServices)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>discoverServices (peripheralUuid, uuids)](#apidoc.element.noble.noble.prototype.discoverServices)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>notify (peripheralUuid, serviceUuid, characteristicUuid, notify)](#apidoc.element.noble.noble.prototype.notify)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onAddressChange (address)](#apidoc.element.noble.noble.prototype.onAddressChange)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onBroadcast (peripheralUuid, serviceUuid, characteristicUuid, state)](#apidoc.element.noble.noble.prototype.onBroadcast)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onCharacteristicsDiscover (peripheralUuid, serviceUuid, characteristics)](#apidoc.element.noble.noble.prototype.onCharacteristicsDiscover)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onConnect (peripheralUuid, error)](#apidoc.element.noble.noble.prototype.onConnect)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onDescriptorsDiscover (peripheralUuid, serviceUuid, characteristicUuid, descriptors)](#apidoc.element.noble.noble.prototype.onDescriptorsDiscover)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onDisconnect (peripheralUuid)](#apidoc.element.noble.noble.prototype.onDisconnect)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onDiscover (uuid, address, addressType, connectable, advertisement, rssi)](#apidoc.element.noble.noble.prototype.onDiscover)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onHandleNotify (peripheralUuid, handle, data)](#apidoc.element.noble.noble.prototype.onHandleNotify)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onHandleRead (peripheralUuid, handle, data)](#apidoc.element.noble.noble.prototype.onHandleRead)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onHandleWrite (peripheralUuid, handle)](#apidoc.element.noble.noble.prototype.onHandleWrite)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onIncludedServicesDiscover (peripheralUuid, serviceUuid, includedServiceUuids)](#apidoc.element.noble.noble.prototype.onIncludedServicesDiscover)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onNotify (peripheralUuid, serviceUuid, characteristicUuid, state)](#apidoc.element.noble.noble.prototype.onNotify)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onRead (peripheralUuid, serviceUuid, characteristicUuid, data, isNotification)](#apidoc.element.noble.noble.prototype.onRead)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onRssiUpdate (peripheralUuid, rssi)](#apidoc.element.noble.noble.prototype.onRssiUpdate)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onScanStart (filterDuplicates)](#apidoc.element.noble.noble.prototype.onScanStart)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onScanStop ()](#apidoc.element.noble.noble.prototype.onScanStop)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onServicesDiscover (peripheralUuid, serviceUuids)](#apidoc.element.noble.noble.prototype.onServicesDiscover)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onStateChange (state)](#apidoc.element.noble.noble.prototype.onStateChange)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onValueRead (peripheralUuid, serviceUuid, characteristicUuid, descriptorUuid, data)](#apidoc.element.noble.noble.prototype.onValueRead)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onValueWrite (peripheralUuid, serviceUuid, characteristicUuid, descriptorUuid)](#apidoc.element.noble.noble.prototype.onValueWrite)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onWrite (peripheralUuid, serviceUuid, characteristicUuid)](#apidoc.element.noble.noble.prototype.onWrite)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>read (peripheralUuid, serviceUuid, characteristicUuid)](#apidoc.element.noble.noble.prototype.read)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>readHandle (peripheralUuid, handle)](#apidoc.element.noble.noble.prototype.readHandle)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>readValue (peripheralUuid, serviceUuid, characteristicUuid, descriptorUuid)](#apidoc.element.noble.noble.prototype.readValue)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>startScanning (serviceUuids, allowDuplicates, callback)](#apidoc.element.noble.noble.prototype.startScanning)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>stopScanning (callback)](#apidoc.element.noble.noble.prototype.stopScanning)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>updateRssi (peripheralUuid)](#apidoc.element.noble.noble.prototype.updateRssi)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>write (peripheralUuid, serviceUuid, characteristicUuid, data, withoutResponse)](#apidoc.element.noble.noble.prototype.write)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>writeHandle (peripheralUuid, handle, data, withoutResponse)](#apidoc.element.noble.noble.prototype.writeHandle)
1.  [function <span class="apidocSignatureSpan">noble.noble.prototype.</span>writeValue (peripheralUuid, serviceUuid, characteristicUuid, descriptorUuid, data)](#apidoc.element.noble.noble.prototype.writeValue)

#### [module noble.peripheral](#apidoc.module.noble.peripheral)
1.  [function <span class="apidocSignatureSpan">noble.</span>peripheral (noble, id, address, addressType, connectable, advertisement, rssi)](#apidoc.element.noble.peripheral.peripheral)
1.  [function <span class="apidocSignatureSpan">noble.peripheral.</span>super_ ()](#apidoc.element.noble.peripheral.super_)

#### [module noble.peripheral.prototype](#apidoc.module.noble.peripheral.prototype)
1.  [function <span class="apidocSignatureSpan">noble.peripheral.prototype.</span>connect (callback)](#apidoc.element.noble.peripheral.prototype.connect)
1.  [function <span class="apidocSignatureSpan">noble.peripheral.prototype.</span>disconnect (callback)](#apidoc.element.noble.peripheral.prototype.disconnect)
1.  [function <span class="apidocSignatureSpan">noble.peripheral.prototype.</span>discoverAllServicesAndCharacteristics (callback)](#apidoc.element.noble.peripheral.prototype.discoverAllServicesAndCharacteristics)
1.  [function <span class="apidocSignatureSpan">noble.peripheral.prototype.</span>discoverServices (uuids, callback)](#apidoc.element.noble.peripheral.prototype.discoverServices)
1.  [function <span class="apidocSignatureSpan">noble.peripheral.prototype.</span>discoverSomeServicesAndCharacteristics (serviceUuids, characteristicsUuids, callback)](#apidoc.element.noble.peripheral.prototype.discoverSomeServicesAndCharacteristics)
1.  [function <span class="apidocSignatureSpan">noble.peripheral.prototype.</span>readHandle (handle, callback)](#apidoc.element.noble.peripheral.prototype.readHandle)
1.  [function <span class="apidocSignatureSpan">noble.peripheral.prototype.</span>toString ()](#apidoc.element.noble.peripheral.prototype.toString)
1.  [function <span class="apidocSignatureSpan">noble.peripheral.prototype.</span>updateRssi (callback)](#apidoc.element.noble.peripheral.prototype.updateRssi)
1.  [function <span class="apidocSignatureSpan">noble.peripheral.prototype.</span>writeHandle (handle, data, withoutResponse, callback)](#apidoc.element.noble.peripheral.prototype.writeHandle)

#### [module noble.service](#apidoc.module.noble.service)
1.  [function <span class="apidocSignatureSpan">noble.</span>service (noble, peripheralId, uuid)](#apidoc.element.noble.service.service)
1.  [function <span class="apidocSignatureSpan">noble.service.</span>super_ ()](#apidoc.element.noble.service.super_)

#### [module noble.service.prototype](#apidoc.module.noble.service.prototype)
1.  [function <span class="apidocSignatureSpan">noble.service.prototype.</span>discoverCharacteristics (characteristicUuids, callback)](#apidoc.element.noble.service.prototype.discoverCharacteristics)
1.  [function <span class="apidocSignatureSpan">noble.service.prototype.</span>discoverIncludedServices (serviceUuids, callback)](#apidoc.element.noble.service.prototype.discoverIncludedServices)
1.  [function <span class="apidocSignatureSpan">noble.service.prototype.</span>toString ()](#apidoc.element.noble.service.prototype.toString)



# <a name="apidoc.module.noble"></a>[module noble](#apidoc.module.noble)

#### <a name="apidoc.element.noble.noble"></a>[function <span class="apidocSignatureSpan"></span>noble (bindings)](#apidoc.element.noble.noble)
- description and source-code
```javascript
function Noble(bindings) {
  this.state = 'unknown';
  this.address = 'unknown';

  this._bindings = bindings;
  this._peripherals = {};
  this._services = {};
  this._characteristics = {};
  this._descriptors = {};
  this._discoveredPeripheralUUids = [];

  this._bindings.on('stateChange', this.onStateChange.bind(this));
  this._bindings.on('addressChange', this.onAddressChange.bind(this));
  this._bindings.on('scanStart', this.onScanStart.bind(this));
  this._bindings.on('scanStop', this.onScanStop.bind(this));
  this._bindings.on('discover', this.onDiscover.bind(this));
  this._bindings.on('connect', this.onConnect.bind(this));
  this._bindings.on('disconnect', this.onDisconnect.bind(this));
  this._bindings.on('rssiUpdate', this.onRssiUpdate.bind(this));
  this._bindings.on('servicesDiscover', this.onServicesDiscover.bind(this));
  this._bindings.on('includedServicesDiscover', this.onIncludedServicesDiscover.bind(this));
  this._bindings.on('characteristicsDiscover', this.onCharacteristicsDiscover.bind(this));
  this._bindings.on('read', this.onRead.bind(this));
  this._bindings.on('write', this.onWrite.bind(this));
  this._bindings.on('broadcast', this.onBroadcast.bind(this));
  this._bindings.on('notify', this.onNotify.bind(this));
  this._bindings.on('descriptorsDiscover', this.onDescriptorsDiscover.bind(this));
  this._bindings.on('valueRead', this.onValueRead.bind(this));
  this._bindings.on('valueWrite', this.onValueWrite.bind(this));
  this._bindings.on('handleRead', this.onHandleRead.bind(this));
  this._bindings.on('handleWrite', this.onHandleWrite.bind(this));
  this._bindings.on('handleNotify', this.onHandleNotify.bind(this));

  this.on('warning', function(message) {
    if (this.listeners('warning').length === 1) {
      console.warn('noble: ' + message);
    }
  }.bind(this));

  this._bindings.init();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.characteristic"></a>[function <span class="apidocSignatureSpan">noble.</span>characteristic (noble, peripheralId, serviceUuid, uuid, properties)](#apidoc.element.noble.characteristic)
- description and source-code
```javascript
function Characteristic(noble, peripheralId, serviceUuid, uuid, properties) {
  this._noble = noble;
  this._peripheralId = peripheralId;
  this._serviceUuid = serviceUuid;

  this.uuid = uuid;
  this.name = null;
  this.type = null;
  this.properties = properties;
  this.descriptors = null;

  var characteristic = characteristics[uuid];
  if (characteristic) {
    this.name = characteristic.name;
    this.type = characteristic.type;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.descriptor"></a>[function <span class="apidocSignatureSpan">noble.</span>descriptor (noble, peripheralId, serviceUuid, characteristicUuid, uuid)](#apidoc.element.noble.descriptor)
- description and source-code
```javascript
function Descriptor(noble, peripheralId, serviceUuid, characteristicUuid, uuid) {
  this._noble = noble;
  this._peripheralId = peripheralId;
  this._serviceUuid = serviceUuid;
  this._characteristicUuid = characteristicUuid;

  this.uuid = uuid;
  this.name = null;
  this.type = null;

  var descriptor = descriptors[uuid];
  if (descriptor) {
    this.name = descriptor.name;
    this.type = descriptor.type;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.peripheral"></a>[function <span class="apidocSignatureSpan">noble.</span>peripheral (noble, id, address, addressType, connectable, advertisement, rssi)](#apidoc.element.noble.peripheral)
- description and source-code
```javascript
function Peripheral(noble, id, address, addressType, connectable, advertisement, rssi) {
  this._noble = noble;

  this.id = id;
  this.uuid = id; // for legacy
  this.address = address;
  this.addressType = addressType;
  this.connectable = connectable;
  this.advertisement = advertisement;
  this.rssi = rssi;
  this.services = null;
  this.state = 'disconnected';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.service"></a>[function <span class="apidocSignatureSpan">noble.</span>service (noble, peripheralId, uuid)](#apidoc.element.noble.service)
- description and source-code
```javascript
function Service(noble, peripheralId, uuid) {
  this._noble = noble;
  this._peripheralId = peripheralId;

  this.uuid = uuid;
  this.name = null;
  this.type = null;
  this.includedServiceUuids = null;
  this.characteristics = null;

  var service = services[uuid];
  if (service) {
    this.name = service.name;
    this.type = service.type;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.noble._bindings"></a>[module noble._bindings](#apidoc.module.noble._bindings)

#### <a name="apidoc.element.noble._bindings.onSigIntBinded"></a>[function <span class="apidocSignatureSpan">noble._bindings.</span>onSigIntBinded ()](#apidoc.element.noble._bindings.onSigIntBinded)
- description and source-code
```javascript
onSigIntBinded = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.noble._bindings._events"></a>[module noble._bindings._events](#apidoc.module.noble._bindings._events)

#### <a name="apidoc.element.noble._bindings._events.addressChange"></a>[function <span class="apidocSignatureSpan">noble._bindings._events.</span>addressChange ()](#apidoc.element.noble._bindings._events.addressChange)
- description and source-code
```javascript
addressChange = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble._bindings._events.broadcast"></a>[function <span class="apidocSignatureSpan">noble._bindings._events.</span>broadcast ()](#apidoc.element.noble._bindings._events.broadcast)
- description and source-code
```javascript
broadcast = function () { [native code] }
```
- example usage
```shell
...
* '''withoutResponse''':
  * '''false''': send a write request, used with "write" characteristic property
  * '''true''': send a write command, used with "write without response" characteristic property

##### Broadcast

'''javascript
characteristic.broadcast(broadcast[, callback(error)]); // broadcast is true|false
'''

##### Subscribe

'''javascript
characteristic.subscribe([callback(error)]);
'''
...
```

#### <a name="apidoc.element.noble._bindings._events.characteristicsDiscover"></a>[function <span class="apidocSignatureSpan">noble._bindings._events.</span>characteristicsDiscover ()](#apidoc.element.noble._bindings._events.characteristicsDiscover)
- description and source-code
```javascript
characteristicsDiscover = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble._bindings._events.connect"></a>[function <span class="apidocSignatureSpan">noble._bindings._events.</span>connect ()](#apidoc.element.noble._bindings._events.connect)
- description and source-code
```javascript
connect = function () { [native code] }
```
- example usage
```shell
...
'''

#### Peripheral

##### Connect

'''javascript
peripheral.connect([callback(error)]);
'''

##### Disconnect or cancel pending connection

'''javascript
peripheral.disconnect([callback(error)]);
'''
...
```

#### <a name="apidoc.element.noble._bindings._events.descriptorsDiscover"></a>[function <span class="apidocSignatureSpan">noble._bindings._events.</span>descriptorsDiscover ()](#apidoc.element.noble._bindings._events.descriptorsDiscover)
- description and source-code
```javascript
descriptorsDiscover = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble._bindings._events.disconnect"></a>[function <span class="apidocSignatureSpan">noble._bindings._events.</span>disconnect ()](#apidoc.element.noble._bindings._events.disconnect)
- description and source-code
```javascript
disconnect = function () { [native code] }
```
- example usage
```shell
...
'''javascript
peripheral.connect([callback(error)]);
'''

##### Disconnect or cancel pending connection

'''javascript
peripheral.disconnect([callback(error)]);
'''

##### Update RSSI

'''javascript
peripheral.updateRssi([callback(error, rssi)]);
'''
...
```

#### <a name="apidoc.element.noble._bindings._events.discover"></a>[function <span class="apidocSignatureSpan">noble._bindings._events.</span>discover ()](#apidoc.element.noble._bindings._events.discover)
- description and source-code
```javascript
discover = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble._bindings._events.handleNotify"></a>[function <span class="apidocSignatureSpan">noble._bindings._events.</span>handleNotify ()](#apidoc.element.noble._bindings._events.handleNotify)
- description and source-code
```javascript
handleNotify = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble._bindings._events.handleRead"></a>[function <span class="apidocSignatureSpan">noble._bindings._events.</span>handleRead ()](#apidoc.element.noble._bindings._events.handleRead)
- description and source-code
```javascript
handleRead = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble._bindings._events.handleWrite"></a>[function <span class="apidocSignatureSpan">noble._bindings._events.</span>handleWrite ()](#apidoc.element.noble._bindings._events.handleWrite)
- description and source-code
```javascript
handleWrite = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble._bindings._events.includedServicesDiscover"></a>[function <span class="apidocSignatureSpan">noble._bindings._events.</span>includedServicesDiscover ()](#apidoc.element.noble._bindings._events.includedServicesDiscover)
- description and source-code
```javascript
includedServicesDiscover = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble._bindings._events.notify"></a>[function <span class="apidocSignatureSpan">noble._bindings._events.</span>notify ()](#apidoc.element.noble._bindings._events.notify)
- description and source-code
```javascript
notify = function () { [native code] }
```
- example usage
```shell
...

'''javascript
characteristic.once('broadcast', callback(state));
'''

##### Notify

Emitted when characteristic notification state changes, result of '''characteristic.notify(...)'''.

'''javascript
characteristic.once('notify', callback(state));
'''

##### Descriptors discovered
...
```

#### <a name="apidoc.element.noble._bindings._events.read"></a>[function <span class="apidocSignatureSpan">noble._bindings._events.</span>read ()](#apidoc.element.noble._bindings._events.read)
- description and source-code
```javascript
read = function () { [native code] }
```
- example usage
```shell
...
'''

#### Characteristic

##### Read

'''javascript
characteristic.read([callback(error, data)]);
'''

##### Write

'''javascript
characteristic.write(data, withoutResponse[, callback(error)]); // data is a buffer, withoutResponse is true|false
'''
...
```

#### <a name="apidoc.element.noble._bindings._events.rssiUpdate"></a>[function <span class="apidocSignatureSpan">noble._bindings._events.</span>rssiUpdate ()](#apidoc.element.noble._bindings._events.rssiUpdate)
- description and source-code
```javascript
rssiUpdate = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble._bindings._events.scanStart"></a>[function <span class="apidocSignatureSpan">noble._bindings._events.</span>scanStart ()](#apidoc.element.noble._bindings._events.scanStart)
- description and source-code
```javascript
scanStart = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble._bindings._events.scanStop"></a>[function <span class="apidocSignatureSpan">noble._bindings._events.</span>scanStop ()](#apidoc.element.noble._bindings._events.scanStop)
- description and source-code
```javascript
scanStop = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble._bindings._events.servicesDiscover"></a>[function <span class="apidocSignatureSpan">noble._bindings._events.</span>servicesDiscover ()](#apidoc.element.noble._bindings._events.servicesDiscover)
- description and source-code
```javascript
servicesDiscover = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble._bindings._events.stateChange"></a>[function <span class="apidocSignatureSpan">noble._bindings._events.</span>stateChange ()](#apidoc.element.noble._bindings._events.stateChange)
- description and source-code
```javascript
stateChange = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble._bindings._events.valueRead"></a>[function <span class="apidocSignatureSpan">noble._bindings._events.</span>valueRead ()](#apidoc.element.noble._bindings._events.valueRead)
- description and source-code
```javascript
valueRead = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble._bindings._events.valueWrite"></a>[function <span class="apidocSignatureSpan">noble._bindings._events.</span>valueWrite ()](#apidoc.element.noble._bindings._events.valueWrite)
- description and source-code
```javascript
valueWrite = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble._bindings._events.write"></a>[function <span class="apidocSignatureSpan">noble._bindings._events.</span>write ()](#apidoc.element.noble._bindings._events.write)
- description and source-code
```javascript
write = function () { [native code] }
```
- example usage
```shell
...
'''javascript
characteristic.read([callback(error, data)]);
'''

##### Write

'''javascript
characteristic.write(data, withoutResponse[, callback(error)]); // data is a buffer, withoutResponse is true|false
'''

* '''withoutResponse''':
  * '''false''': send a write request, used with "write" characteristic property
  * '''true''': send a write command, used with "write without response" characteristic property

##### Broadcast
...
```



# <a name="apidoc.module.noble._events"></a>[module noble._events](#apidoc.module.noble._events)

#### <a name="apidoc.element.noble._events.warning"></a>[function <span class="apidocSignatureSpan">noble._events.</span>warning ()](#apidoc.element.noble._events.warning)
- description and source-code
```javascript
warning = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.noble.characteristic"></a>[module noble.characteristic](#apidoc.module.noble.characteristic)

#### <a name="apidoc.element.noble.characteristic.characteristic"></a>[function <span class="apidocSignatureSpan">noble.</span>characteristic (noble, peripheralId, serviceUuid, uuid, properties)](#apidoc.element.noble.characteristic.characteristic)
- description and source-code
```javascript
function Characteristic(noble, peripheralId, serviceUuid, uuid, properties) {
  this._noble = noble;
  this._peripheralId = peripheralId;
  this._serviceUuid = serviceUuid;

  this.uuid = uuid;
  this.name = null;
  this.type = null;
  this.properties = properties;
  this.descriptors = null;

  var characteristic = characteristics[uuid];
  if (characteristic) {
    this.name = characteristic.name;
    this.type = characteristic.type;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.characteristic.super_"></a>[function <span class="apidocSignatureSpan">noble.characteristic.</span>super_ ()](#apidoc.element.noble.characteristic.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.noble.characteristic.prototype"></a>[module noble.characteristic.prototype](#apidoc.module.noble.characteristic.prototype)

#### <a name="apidoc.element.noble.characteristic.prototype.broadcast"></a>[function <span class="apidocSignatureSpan">noble.characteristic.prototype.</span>broadcast (broadcast, callback)](#apidoc.element.noble.characteristic.prototype.broadcast)
- description and source-code
```javascript
broadcast = function (broadcast, callback) {
  if (callback) {
    this.once('broadcast', function() {
      callback(null);
    });
  }

  this._noble.broadcast(
    this._peripheralId,
    this._serviceUuid,
    this.uuid,
    broadcast
  );
}
```
- example usage
```shell
...
* '''withoutResponse''':
  * '''false''': send a write request, used with "write" characteristic property
  * '''true''': send a write command, used with "write without response" characteristic property

##### Broadcast

'''javascript
characteristic.broadcast(broadcast[, callback(error)]); // broadcast is true|false
'''

##### Subscribe

'''javascript
characteristic.subscribe([callback(error)]);
'''
...
```

#### <a name="apidoc.element.noble.characteristic.prototype.discoverDescriptors"></a>[function <span class="apidocSignatureSpan">noble.characteristic.prototype.</span>discoverDescriptors (callback)](#apidoc.element.noble.characteristic.prototype.discoverDescriptors)
- description and source-code
```javascript
discoverDescriptors = function (callback) {
  if (callback) {
    this.once('descriptorsDiscover', function(descriptors) {
      callback(null, descriptors);
    });
  }

  this._noble.discoverDescriptors(
    this._peripheralId,
    this._serviceUuid,
    this.uuid
  );
}
```
- example usage
```shell
...

  * unsubscribe to a characteristic
  * use for characteristics with notify or indicate properties

##### Discover descriptors

'''javascript
characteristic.discoverDescriptors([callback(error, descriptors)]);
'''

##### Read value

'''javascript
descriptor.readValue([callback(error, data)]);
'''
...
```

#### <a name="apidoc.element.noble.characteristic.prototype.notify"></a>[function <span class="apidocSignatureSpan">noble.characteristic.prototype.</span>notify (notify, callback)](#apidoc.element.noble.characteristic.prototype.notify)
- description and source-code
```javascript
notify = function (notify, callback) {
  if (callback) {
    this.once('notify', function() {
      callback(null);
    });
  }

  this._noble.notify(
    this._peripheralId,
    this._serviceUuid,
    this.uuid,
    notify
  );
}
```
- example usage
```shell
...

'''javascript
characteristic.once('broadcast', callback(state));
'''

##### Notify

Emitted when characteristic notification state changes, result of '''characteristic.notify(...)'''.

'''javascript
characteristic.once('notify', callback(state));
'''

##### Descriptors discovered
...
```

#### <a name="apidoc.element.noble.characteristic.prototype.read"></a>[function <span class="apidocSignatureSpan">noble.characteristic.prototype.</span>read (callback)](#apidoc.element.noble.characteristic.prototype.read)
- description and source-code
```javascript
read = function (callback) {
  if (callback) {
    this.once('read', function(data) {
      callback(null, data);
    });
  }

  this._noble.read(
    this._peripheralId,
    this._serviceUuid,
    this.uuid
  );
}
```
- example usage
```shell
...
'''

#### Characteristic

##### Read

'''javascript
characteristic.read([callback(error, data)]);
'''

##### Write

'''javascript
characteristic.write(data, withoutResponse[, callback(error)]); // data is a buffer, withoutResponse is true|false
'''
...
```

#### <a name="apidoc.element.noble.characteristic.prototype.subscribe"></a>[function <span class="apidocSignatureSpan">noble.characteristic.prototype.</span>subscribe (callback)](#apidoc.element.noble.characteristic.prototype.subscribe)
- description and source-code
```javascript
subscribe = function (callback) {
  this.notify(true, callback);
}
```
- example usage
```shell
...
'''javascript
characteristic.broadcast(broadcast[, callback(error)]); // broadcast is true|false
'''

##### Subscribe

'''javascript
characteristic.subscribe([callback(error)]);
'''

  * subscribe to a characteristic, triggers ''data'' events when peripheral sends an notification or indication
  * use for characteristics with notify or indicate properties

##### Unsubscribe
...
```

#### <a name="apidoc.element.noble.characteristic.prototype.toString"></a>[function <span class="apidocSignatureSpan">noble.characteristic.prototype.</span>toString ()](#apidoc.element.noble.characteristic.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return JSON.stringify({
    uuid: this.uuid,
    name: this.name,
    type: this.type,
    properties: this.properties
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.characteristic.prototype.unsubscribe"></a>[function <span class="apidocSignatureSpan">noble.characteristic.prototype.</span>unsubscribe (callback)](#apidoc.element.noble.characteristic.prototype.unsubscribe)
- description and source-code
```javascript
unsubscribe = function (callback) {
  this.notify(false, callback);
}
```
- example usage
```shell
...

  * subscribe to a characteristic, triggers ''data'' events when peripheral sends an notification or indication
  * use for characteristics with notify or indicate properties

##### Unsubscribe

'''javascript
characteristic.unsubscribe([callback(error)]);
'''

  * unsubscribe to a characteristic
  * use for characteristics with notify or indicate properties

##### Discover descriptors
...
```

#### <a name="apidoc.element.noble.characteristic.prototype.write"></a>[function <span class="apidocSignatureSpan">noble.characteristic.prototype.</span>write (data, withoutResponse, callback)](#apidoc.element.noble.characteristic.prototype.write)
- description and source-code
```javascript
write = function (data, withoutResponse, callback) {
  if (process.title !== 'browser') {
    if (!(data instanceof Buffer)) {
      throw new Error('data must be a Buffer');
    }
  }

  if (callback) {
    this.once('write', function() {
      callback(null);
    });
  }

  this._noble.write(
    this._peripheralId,
    this._serviceUuid,
    this.uuid,
    data,
    withoutResponse
  );
}
```
- example usage
```shell
...
'''javascript
characteristic.read([callback(error, data)]);
'''

##### Write

'''javascript
characteristic.write(data, withoutResponse[, callback(error)]); // data is a buffer, withoutResponse is true|false
'''

* '''withoutResponse''':
  * '''false''': send a write request, used with "write" characteristic property
  * '''true''': send a write command, used with "write without response" characteristic property

##### Broadcast
...
```



# <a name="apidoc.module.noble.descriptor"></a>[module noble.descriptor](#apidoc.module.noble.descriptor)

#### <a name="apidoc.element.noble.descriptor.descriptor"></a>[function <span class="apidocSignatureSpan">noble.</span>descriptor (noble, peripheralId, serviceUuid, characteristicUuid, uuid)](#apidoc.element.noble.descriptor.descriptor)
- description and source-code
```javascript
function Descriptor(noble, peripheralId, serviceUuid, characteristicUuid, uuid) {
  this._noble = noble;
  this._peripheralId = peripheralId;
  this._serviceUuid = serviceUuid;
  this._characteristicUuid = characteristicUuid;

  this.uuid = uuid;
  this.name = null;
  this.type = null;

  var descriptor = descriptors[uuid];
  if (descriptor) {
    this.name = descriptor.name;
    this.type = descriptor.type;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.descriptor.super_"></a>[function <span class="apidocSignatureSpan">noble.descriptor.</span>super_ ()](#apidoc.element.noble.descriptor.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.noble.descriptor.prototype"></a>[module noble.descriptor.prototype](#apidoc.module.noble.descriptor.prototype)

#### <a name="apidoc.element.noble.descriptor.prototype.readValue"></a>[function <span class="apidocSignatureSpan">noble.descriptor.prototype.</span>readValue (callback)](#apidoc.element.noble.descriptor.prototype.readValue)
- description and source-code
```javascript
readValue = function (callback) {
  if (callback) {
    this.once('valueRead', function(data) {
      callback(null, data);
    });
  }
  this._noble.readValue(
    this._peripheralId,
    this._serviceUuid,
    this._characteristicUuid,
    this.uuid
  );
}
```
- example usage
```shell
...
'''javascript
characteristic.discoverDescriptors([callback(error, descriptors)]);
'''

##### Read value

'''javascript
descriptor.readValue([callback(error, data)]);
'''

##### Write value

'''javascript
descriptor.writeValue(data[, callback(error)]); // data is a buffer
'''
...
```

#### <a name="apidoc.element.noble.descriptor.prototype.toString"></a>[function <span class="apidocSignatureSpan">noble.descriptor.prototype.</span>toString ()](#apidoc.element.noble.descriptor.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return JSON.stringify({
    uuid: this.uuid,
    name: this.name,
    type: this.type
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.descriptor.prototype.writeValue"></a>[function <span class="apidocSignatureSpan">noble.descriptor.prototype.</span>writeValue (data, callback)](#apidoc.element.noble.descriptor.prototype.writeValue)
- description and source-code
```javascript
writeValue = function (data, callback) {
  if (!(data instanceof Buffer)) {
    throw new Error('data must be a Buffer');
  }

  if (callback) {
    this.once('valueWrite', function() {
      callback(null);
    });
  }
  this._noble.writeValue(
    this._peripheralId,
    this._serviceUuid,
    this._characteristicUuid,
    this.uuid,
    data
  );
}
```
- example usage
```shell
...
'''javascript
descriptor.readValue([callback(error, data)]);
'''

##### Write value

'''javascript
descriptor.writeValue(data[, callback(error)]); // data is a buffer
'''

#### Handle

##### Read

'''javascript
...
```



# <a name="apidoc.module.noble.noble"></a>[module noble.noble](#apidoc.module.noble.noble)

#### <a name="apidoc.element.noble.noble.noble"></a>[function <span class="apidocSignatureSpan">noble.</span>noble (bindings)](#apidoc.element.noble.noble.noble)
- description and source-code
```javascript
function Noble(bindings) {
  this.state = 'unknown';
  this.address = 'unknown';

  this._bindings = bindings;
  this._peripherals = {};
  this._services = {};
  this._characteristics = {};
  this._descriptors = {};
  this._discoveredPeripheralUUids = [];

  this._bindings.on('stateChange', this.onStateChange.bind(this));
  this._bindings.on('addressChange', this.onAddressChange.bind(this));
  this._bindings.on('scanStart', this.onScanStart.bind(this));
  this._bindings.on('scanStop', this.onScanStop.bind(this));
  this._bindings.on('discover', this.onDiscover.bind(this));
  this._bindings.on('connect', this.onConnect.bind(this));
  this._bindings.on('disconnect', this.onDisconnect.bind(this));
  this._bindings.on('rssiUpdate', this.onRssiUpdate.bind(this));
  this._bindings.on('servicesDiscover', this.onServicesDiscover.bind(this));
  this._bindings.on('includedServicesDiscover', this.onIncludedServicesDiscover.bind(this));
  this._bindings.on('characteristicsDiscover', this.onCharacteristicsDiscover.bind(this));
  this._bindings.on('read', this.onRead.bind(this));
  this._bindings.on('write', this.onWrite.bind(this));
  this._bindings.on('broadcast', this.onBroadcast.bind(this));
  this._bindings.on('notify', this.onNotify.bind(this));
  this._bindings.on('descriptorsDiscover', this.onDescriptorsDiscover.bind(this));
  this._bindings.on('valueRead', this.onValueRead.bind(this));
  this._bindings.on('valueWrite', this.onValueWrite.bind(this));
  this._bindings.on('handleRead', this.onHandleRead.bind(this));
  this._bindings.on('handleWrite', this.onHandleWrite.bind(this));
  this._bindings.on('handleNotify', this.onHandleNotify.bind(this));

  this.on('warning', function(message) {
    if (this.listeners('warning').length === 1) {
      console.warn('noble: ' + message);
    }
  }.bind(this));

  this._bindings.init();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.noble.super_"></a>[function <span class="apidocSignatureSpan">noble.noble.</span>super_ ()](#apidoc.element.noble.noble.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.noble.noble.prototype"></a>[module noble.noble.prototype](#apidoc.module.noble.noble.prototype)

#### <a name="apidoc.element.noble.noble.prototype.broadcast"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>broadcast (peripheralUuid, serviceUuid, characteristicUuid, broadcast)](#apidoc.element.noble.noble.prototype.broadcast)
- description and source-code
```javascript
broadcast = function (peripheralUuid, serviceUuid, characteristicUuid, broadcast) {
   this._bindings.broadcast(peripheralUuid, serviceUuid, characteristicUuid, broadcast);
}
```
- example usage
```shell
...
* '''withoutResponse''':
  * '''false''': send a write request, used with "write" characteristic property
  * '''true''': send a write command, used with "write without response" characteristic property

##### Broadcast

'''javascript
characteristic.broadcast(broadcast[, callback(error)]); // broadcast is true|false
'''

##### Subscribe

'''javascript
characteristic.subscribe([callback(error)]);
'''
...
```

#### <a name="apidoc.element.noble.noble.prototype.connect"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>connect (peripheralUuid)](#apidoc.element.noble.noble.prototype.connect)
- description and source-code
```javascript
connect = function (peripheralUuid) {
  this._bindings.connect(peripheralUuid);
}
```
- example usage
```shell
...
'''

#### Peripheral

##### Connect

'''javascript
peripheral.connect([callback(error)]);
'''

##### Disconnect or cancel pending connection

'''javascript
peripheral.disconnect([callback(error)]);
'''
...
```

#### <a name="apidoc.element.noble.noble.prototype.disconnect"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>disconnect (peripheralUuid)](#apidoc.element.noble.noble.prototype.disconnect)
- description and source-code
```javascript
disconnect = function (peripheralUuid) {
  this._bindings.disconnect(peripheralUuid);
}
```
- example usage
```shell
...
'''javascript
peripheral.connect([callback(error)]);
'''

##### Disconnect or cancel pending connection

'''javascript
peripheral.disconnect([callback(error)]);
'''

##### Update RSSI

'''javascript
peripheral.updateRssi([callback(error, rssi)]);
'''
...
```

#### <a name="apidoc.element.noble.noble.prototype.discoverCharacteristics"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>discoverCharacteristics (peripheralUuid, serviceUuid, characteristicUuids)](#apidoc.element.noble.noble.prototype.discoverCharacteristics)
- description and source-code
```javascript
discoverCharacteristics = function (peripheralUuid, serviceUuid, characteristicUuids) {
  this._bindings.discoverCharacteristics(peripheralUuid, serviceUuid, characteristicUuids);
}
```
- example usage
```shell
...
var serviceUUIDs = ["<service UUID 1>", ...];
service.discoverIncludedServices(serviceUUIDs[, callback(error, includedServiceUuids)]); // particular UUID's
'''

##### Discover characteristics

'''javascript
service.discoverCharacteristics() // any characteristic UUID

var characteristicUUIDs = ["<characteristic UUID 1>", ...];
service.discoverCharacteristics(characteristicUUIDs[, callback(error, characteristics)]); // particular UUID's
'''

#### Characteristic
...
```

#### <a name="apidoc.element.noble.noble.prototype.discoverDescriptors"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>discoverDescriptors (peripheralUuid, serviceUuid, characteristicUuid)](#apidoc.element.noble.noble.prototype.discoverDescriptors)
- description and source-code
```javascript
discoverDescriptors = function (peripheralUuid, serviceUuid, characteristicUuid) {
  this._bindings.discoverDescriptors(peripheralUuid, serviceUuid, characteristicUuid);
}
```
- example usage
```shell
...

  * unsubscribe to a characteristic
  * use for characteristics with notify or indicate properties

##### Discover descriptors

'''javascript
characteristic.discoverDescriptors([callback(error, descriptors)]);
'''

##### Read value

'''javascript
descriptor.readValue([callback(error, data)]);
'''
...
```

#### <a name="apidoc.element.noble.noble.prototype.discoverIncludedServices"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>discoverIncludedServices (peripheralUuid, serviceUuid, serviceUuids)](#apidoc.element.noble.noble.prototype.discoverIncludedServices)
- description and source-code
```javascript
discoverIncludedServices = function (peripheralUuid, serviceUuid, serviceUuids) {
  this._bindings.discoverIncludedServices(peripheralUuid, serviceUuid, serviceUuids);
}
```
- example usage
```shell
...
peripheral.discoverSomeServicesAndCharacteristics(serviceUUIDs, characteristicUUIDs, [callback(error, services, characteristics));
'''
#### Service

##### Discover included services

'''javascript
service.discoverIncludedServices(); // any service UUID

var serviceUUIDs = ["<service UUID 1>", ...];
service.discoverIncludedServices(serviceUUIDs[, callback(error, includedServiceUuids)]); // particular UUID's
'''

##### Discover characteristics
...
```

#### <a name="apidoc.element.noble.noble.prototype.discoverServices"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>discoverServices (peripheralUuid, uuids)](#apidoc.element.noble.noble.prototype.discoverServices)
- description and source-code
```javascript
discoverServices = function (peripheralUuid, uuids) {
  this._bindings.discoverServices(peripheralUuid, uuids);
}
```
- example usage
```shell
...
'''javascript
peripheral.updateRssi([callback(error, rssi)]);
'''

##### Discover services

'''javascript
peripheral.discoverServices(); // any service UUID

var serviceUUIDs = ["<service UUID 1>", ...];
peripheral.discoverServices(serviceUUIDs[, callback(error, services)]); // particular UUID's
'''

##### Discover all services and characteristics
...
```

#### <a name="apidoc.element.noble.noble.prototype.notify"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>notify (peripheralUuid, serviceUuid, characteristicUuid, notify)](#apidoc.element.noble.noble.prototype.notify)
- description and source-code
```javascript
notify = function (peripheralUuid, serviceUuid, characteristicUuid, notify) {
   this._bindings.notify(peripheralUuid, serviceUuid, characteristicUuid, notify);
}
```
- example usage
```shell
...

'''javascript
characteristic.once('broadcast', callback(state));
'''

##### Notify

Emitted when characteristic notification state changes, result of '''characteristic.notify(...)'''.

'''javascript
characteristic.once('notify', callback(state));
'''

##### Descriptors discovered
...
```

#### <a name="apidoc.element.noble.noble.prototype.onAddressChange"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onAddressChange (address)](#apidoc.element.noble.noble.prototype.onAddressChange)
- description and source-code
```javascript
onAddressChange = function (address) {
  debug('addressChange ' + address);

  this.address = address;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.noble.prototype.onBroadcast"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onBroadcast (peripheralUuid, serviceUuid, characteristicUuid, state)](#apidoc.element.noble.noble.prototype.onBroadcast)
- description and source-code
```javascript
onBroadcast = function (peripheralUuid, serviceUuid, characteristicUuid, state) {
  var characteristic = this._characteristics[peripheralUuid][serviceUuid][characteristicUuid];

  if (characteristic) {
    characteristic.emit('broadcast', state);
  } else {
    this.emit('warning', 'unknown peripheral ' + peripheralUuid + ', ' + serviceUuid + ', ' + characteristicUuid + ' broadcast!');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.noble.prototype.onCharacteristicsDiscover"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onCharacteristicsDiscover (peripheralUuid, serviceUuid, characteristics)](#apidoc.element.noble.noble.prototype.onCharacteristicsDiscover)
- description and source-code
```javascript
onCharacteristicsDiscover = function (peripheralUuid, serviceUuid, characteristics) {
  var service = this._services[peripheralUuid][serviceUuid];

  if (service) {
    var characteristics_ = [];

    for (var i = 0; i < characteristics.length; i++) {
      var characteristicUuid = characteristics[i].uuid;

      var characteristic = new Characteristic(
                                this,
                                peripheralUuid,
                                serviceUuid,
                                characteristicUuid,
                                characteristics[i].properties
                            );

      this._characteristics[peripheralUuid][serviceUuid][characteristicUuid] = characteristic;
      this._descriptors[peripheralUuid][serviceUuid][characteristicUuid] = {};

      characteristics_.push(characteristic);
    }

    service.characteristics = characteristics_;

    service.emit('characteristicsDiscover', characteristics_);
  } else {
    this.emit('warning', 'unknown peripheral ' + peripheralUuid + ', ' + serviceUuid + ' characteristics discover!');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.noble.prototype.onConnect"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onConnect (peripheralUuid, error)](#apidoc.element.noble.noble.prototype.onConnect)
- description and source-code
```javascript
onConnect = function (peripheralUuid, error) {
  var peripheral = this._peripherals[peripheralUuid];

  if (peripheral) {
    peripheral.state = error ? 'error' : 'connected';
    peripheral.emit('connect', error);
  } else {
    this.emit('warning', 'unknown peripheral ' + peripheralUuid + ' connected!');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.noble.prototype.onDescriptorsDiscover"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onDescriptorsDiscover (peripheralUuid, serviceUuid, characteristicUuid, descriptors)](#apidoc.element.noble.noble.prototype.onDescriptorsDiscover)
- description and source-code
```javascript
onDescriptorsDiscover = function (peripheralUuid, serviceUuid, characteristicUuid, descriptors) {
  var characteristic = this._characteristics[peripheralUuid][serviceUuid][characteristicUuid];

  if (characteristic) {
    var descriptors_ = [];

    for (var i = 0; i < descriptors.length; i++) {
      var descriptorUuid = descriptors[i];

      var descriptor = new Descriptor(
                            this,
                            peripheralUuid,
                            serviceUuid,
                            characteristicUuid,
                            descriptorUuid
                        );

      this._descriptors[peripheralUuid][serviceUuid][characteristicUuid][descriptorUuid] = descriptor;

      descriptors_.push(descriptor);
    }

    characteristic.descriptors = descriptors_;

    characteristic.emit('descriptorsDiscover', descriptors_);
  } else {
    this.emit('warning', 'unknown peripheral ' + peripheralUuid + ', ' + serviceUuid + ', ' + characteristicUuid + ' descriptors
 discover!');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.noble.prototype.onDisconnect"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onDisconnect (peripheralUuid)](#apidoc.element.noble.noble.prototype.onDisconnect)
- description and source-code
```javascript
onDisconnect = function (peripheralUuid) {
  var peripheral = this._peripherals[peripheralUuid];

  if (peripheral) {
    peripheral.state = 'disconnected';
    peripheral.emit('disconnect');
  } else {
    this.emit('warning', 'unknown peripheral ' + peripheralUuid + ' disconnected!');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.noble.prototype.onDiscover"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onDiscover (uuid, address, addressType, connectable, advertisement, rssi)](#apidoc.element.noble.noble.prototype.onDiscover)
- description and source-code
```javascript
onDiscover = function (uuid, address, addressType, connectable, advertisement, rssi) {
  var peripheral = this._peripherals[uuid];

  if (!peripheral) {
    peripheral = new Peripheral(this, uuid, address, addressType, connectable, advertisement, rssi);

    this._peripherals[uuid] = peripheral;
    this._services[uuid] = {};
    this._characteristics[uuid] = {};
    this._descriptors[uuid] = {};
  } else {
    // "or" the advertisment data with existing
    for (var i in advertisement) {
      if (advertisement[i] !== undefined) {
        peripheral.advertisement[i] = advertisement[i];
      }
    }

    peripheral.rssi = rssi;
  }

  var previouslyDiscoverd = (this._discoveredPeripheralUUids.indexOf(uuid) !== -1);

  if (!previouslyDiscoverd) {
    this._discoveredPeripheralUUids.push(uuid);
  }

  if (this._allowDuplicates || !previouslyDiscoverd) {
    this.emit('discover', peripheral);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.noble.prototype.onHandleNotify"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onHandleNotify (peripheralUuid, handle, data)](#apidoc.element.noble.noble.prototype.onHandleNotify)
- description and source-code
```javascript
onHandleNotify = function (peripheralUuid, handle, data) {
  var peripheral = this._peripherals[peripheralUuid];

  if (peripheral) {
    peripheral.emit('handleNotify', handle, data);
  } else {
    this.emit('warning', 'unknown peripheral ' + peripheralUuid + ' handle notify!');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.noble.prototype.onHandleRead"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onHandleRead (peripheralUuid, handle, data)](#apidoc.element.noble.noble.prototype.onHandleRead)
- description and source-code
```javascript
onHandleRead = function (peripheralUuid, handle, data) {
  var peripheral = this._peripherals[peripheralUuid];

  if (peripheral) {
    peripheral.emit('handleRead' + handle, data);
  } else {
    this.emit('warning', 'unknown peripheral ' + peripheralUuid + ' handle read!');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.noble.prototype.onHandleWrite"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onHandleWrite (peripheralUuid, handle)](#apidoc.element.noble.noble.prototype.onHandleWrite)
- description and source-code
```javascript
onHandleWrite = function (peripheralUuid, handle) {
  var peripheral = this._peripherals[peripheralUuid];

  if (peripheral) {
    peripheral.emit('handleWrite' + handle);
  } else {
    this.emit('warning', 'unknown peripheral ' + peripheralUuid + ' handle write!');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.noble.prototype.onIncludedServicesDiscover"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onIncludedServicesDiscover (peripheralUuid, serviceUuid, includedServiceUuids)](#apidoc.element.noble.noble.prototype.onIncludedServicesDiscover)
- description and source-code
```javascript
onIncludedServicesDiscover = function (peripheralUuid, serviceUuid, includedServiceUuids) {
  var service = this._services[peripheralUuid][serviceUuid];

  if (service) {
    service.includedServiceUuids = includedServiceUuids;

    service.emit('includedServicesDiscover', includedServiceUuids);
  } else {
    this.emit('warning', 'unknown peripheral ' + peripheralUuid + ', ' + serviceUuid + ' included services discover!');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.noble.prototype.onNotify"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onNotify (peripheralUuid, serviceUuid, characteristicUuid, state)](#apidoc.element.noble.noble.prototype.onNotify)
- description and source-code
```javascript
onNotify = function (peripheralUuid, serviceUuid, characteristicUuid, state) {
  var characteristic = this._characteristics[peripheralUuid][serviceUuid][characteristicUuid];

  if (characteristic) {
    characteristic.emit('notify', state);
  } else {
    this.emit('warning', 'unknown peripheral ' + peripheralUuid + ', ' + serviceUuid + ', ' + characteristicUuid + ' notify!');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.noble.prototype.onRead"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onRead (peripheralUuid, serviceUuid, characteristicUuid, data, isNotification)](#apidoc.element.noble.noble.prototype.onRead)
- description and source-code
```javascript
onRead = function (peripheralUuid, serviceUuid, characteristicUuid, data, isNotification) {
  var characteristic = this._characteristics[peripheralUuid][serviceUuid][characteristicUuid];

  if (characteristic) {
    characteristic.emit('data', data, isNotification);

    if (!isNotification) {
      characteristic.emit('read', data, isNotification); // for backwards compatbility
    }
  } else {
    this.emit('warning', 'unknown peripheral ' + peripheralUuid + ', ' + serviceUuid + ', ' + characteristicUuid + ' read!');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.noble.prototype.onRssiUpdate"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onRssiUpdate (peripheralUuid, rssi)](#apidoc.element.noble.noble.prototype.onRssiUpdate)
- description and source-code
```javascript
onRssiUpdate = function (peripheralUuid, rssi) {
  var peripheral = this._peripherals[peripheralUuid];

  if (peripheral) {
    peripheral.rssi = rssi;

    peripheral.emit('rssiUpdate', rssi);
  } else {
    this.emit('warning', 'unknown peripheral ' + peripheralUuid + ' RSSI update!');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.noble.prototype.onScanStart"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onScanStart (filterDuplicates)](#apidoc.element.noble.noble.prototype.onScanStart)
- description and source-code
```javascript
onScanStart = function (filterDuplicates) {
  debug('scanStart');
  this.emit('scanStart', filterDuplicates);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.noble.prototype.onScanStop"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onScanStop ()](#apidoc.element.noble.noble.prototype.onScanStop)
- description and source-code
```javascript
onScanStop = function () {
  debug('scanStop');
  this.emit('scanStop');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.noble.prototype.onServicesDiscover"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onServicesDiscover (peripheralUuid, serviceUuids)](#apidoc.element.noble.noble.prototype.onServicesDiscover)
- description and source-code
```javascript
onServicesDiscover = function (peripheralUuid, serviceUuids) {
  var peripheral = this._peripherals[peripheralUuid];

  if (peripheral) {
    var services = [];

    for (var i = 0; i < serviceUuids.length; i++) {
      var serviceUuid = serviceUuids[i];
      var service = new Service(this, peripheralUuid, serviceUuid);

      this._services[peripheralUuid][serviceUuid] = service;
      this._characteristics[peripheralUuid][serviceUuid] = {};
      this._descriptors[peripheralUuid][serviceUuid] = {};

      services.push(service);
    }

    peripheral.services = services;

    peripheral.emit('servicesDiscover', services);
  } else {
    this.emit('warning', 'unknown peripheral ' + peripheralUuid + ' services discover!');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.noble.prototype.onStateChange"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onStateChange (state)](#apidoc.element.noble.noble.prototype.onStateChange)
- description and source-code
```javascript
onStateChange = function (state) {
  debug('stateChange ' + state);

  this.state = state;

  this.emit('stateChange', state);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.noble.prototype.onValueRead"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onValueRead (peripheralUuid, serviceUuid, characteristicUuid, descriptorUuid, data)](#apidoc.element.noble.noble.prototype.onValueRead)
- description and source-code
```javascript
onValueRead = function (peripheralUuid, serviceUuid, characteristicUuid, descriptorUuid, data) {
  var descriptor = this._descriptors[peripheralUuid][serviceUuid][characteristicUuid][descriptorUuid];

  if (descriptor) {
    descriptor.emit('valueRead', data);
  } else {
    this.emit('warning', 'unknown peripheral ' + peripheralUuid + ', ' + serviceUuid + ', ' + characteristicUuid + ', ' + descriptorUuid
 + ' value read!');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.noble.prototype.onValueWrite"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onValueWrite (peripheralUuid, serviceUuid, characteristicUuid, descriptorUuid)](#apidoc.element.noble.noble.prototype.onValueWrite)
- description and source-code
```javascript
onValueWrite = function (peripheralUuid, serviceUuid, characteristicUuid, descriptorUuid) {
  var descriptor = this._descriptors[peripheralUuid][serviceUuid][characteristicUuid][descriptorUuid];

  if (descriptor) {
    descriptor.emit('valueWrite');
  } else {
    this.emit('warning', 'unknown peripheral ' + peripheralUuid + ', ' + serviceUuid + ', ' + characteristicUuid + ', ' + descriptorUuid
 + ' value write!');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.noble.prototype.onWrite"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>onWrite (peripheralUuid, serviceUuid, characteristicUuid)](#apidoc.element.noble.noble.prototype.onWrite)
- description and source-code
```javascript
onWrite = function (peripheralUuid, serviceUuid, characteristicUuid) {
  var characteristic = this._characteristics[peripheralUuid][serviceUuid][characteristicUuid];

  if (characteristic) {
    characteristic.emit('write');
  } else {
    this.emit('warning', 'unknown peripheral ' + peripheralUuid + ', ' + serviceUuid + ', ' + characteristicUuid + ' write!');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.noble.prototype.read"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>read (peripheralUuid, serviceUuid, characteristicUuid)](#apidoc.element.noble.noble.prototype.read)
- description and source-code
```javascript
read = function (peripheralUuid, serviceUuid, characteristicUuid) {
   this._bindings.read(peripheralUuid, serviceUuid, characteristicUuid);
}
```
- example usage
```shell
...
'''

#### Characteristic

##### Read

'''javascript
characteristic.read([callback(error, data)]);
'''

##### Write

'''javascript
characteristic.write(data, withoutResponse[, callback(error)]); // data is a buffer, withoutResponse is true|false
'''
...
```

#### <a name="apidoc.element.noble.noble.prototype.readHandle"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>readHandle (peripheralUuid, handle)](#apidoc.element.noble.noble.prototype.readHandle)
- description and source-code
```javascript
readHandle = function (peripheralUuid, handle) {
  this._bindings.readHandle(peripheralUuid, handle);
}
```
- example usage
```shell
...
'''

#### Handle

##### Read

'''javascript
peripheral.readHandle(handle, callback(error, data));
'''

##### Write

'''javascript
peripheral.writeHandle(handle, data, withoutResponse, callback(error));
'''
...
```

#### <a name="apidoc.element.noble.noble.prototype.readValue"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>readValue (peripheralUuid, serviceUuid, characteristicUuid, descriptorUuid)](#apidoc.element.noble.noble.prototype.readValue)
- description and source-code
```javascript
readValue = function (peripheralUuid, serviceUuid, characteristicUuid, descriptorUuid) {
  this._bindings.readValue(peripheralUuid, serviceUuid, characteristicUuid, descriptorUuid);
}
```
- example usage
```shell
...
'''javascript
characteristic.discoverDescriptors([callback(error, descriptors)]);
'''

##### Read value

'''javascript
descriptor.readValue([callback(error, data)]);
'''

##### Write value

'''javascript
descriptor.writeValue(data[, callback(error)]); // data is a buffer
'''
...
```

#### <a name="apidoc.element.noble.noble.prototype.startScanning"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>startScanning (serviceUuids, allowDuplicates, callback)](#apidoc.element.noble.noble.prototype.startScanning)
- description and source-code
```javascript
startScanning = function (serviceUuids, allowDuplicates, callback) {
  if (this.state !== 'poweredOn') {
    var error = new Error('Could not start scanning, state is ' + this.state + ' (not poweredOn)');

    if (typeof callback === 'function') {
      callback(error);
    } else {
      throw error;
    }
  } else {
    if (callback) {
      this.once('scanStart', function(filterDuplicates) {
        callback(null, filterDuplicates);
      });
    }

    this._discoveredPeripheralUUids = [];
    this._allowDuplicates = allowDuplicates;

    this._bindings.startScanning(serviceUuids, allowDuplicates);
  }
}
```
- example usage
```shell
...
'''

### Actions

#### Start scanning

'''javascript
noble.startScanning(); // any service UUID, no duplicates


noble.startScanning([], true); // any service UUID, allow duplicates


var serviceUUIDs = ["<service UUID 1>", ...]; // default: [] => all
var allowDuplicates = <false|true>; // default: false
...
```

#### <a name="apidoc.element.noble.noble.prototype.stopScanning"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>stopScanning (callback)](#apidoc.element.noble.noble.prototype.stopScanning)
- description and source-code
```javascript
stopScanning = function (callback) {
  if (callback) {
    this.once('scanStop', callback);
  }
  this._bindings.stopScanning();
}
```
- example usage
```shell
...
'''

__NOTE:__ '''noble.state''' must be '''poweredOn''' before scanning is started. '''noble.on('stateChange', callback(state));'''
can be used register for state change events.

#### Stop scanning

'''javascript
noble.stopScanning();
'''

#### Peripheral

##### Connect

'''javascript
...
```

#### <a name="apidoc.element.noble.noble.prototype.updateRssi"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>updateRssi (peripheralUuid)](#apidoc.element.noble.noble.prototype.updateRssi)
- description and source-code
```javascript
updateRssi = function (peripheralUuid) {
  this._bindings.updateRssi(peripheralUuid);
}
```
- example usage
```shell
...
'''javascript
peripheral.disconnect([callback(error)]);
'''

##### Update RSSI

'''javascript
peripheral.updateRssi([callback(error, rssi)]);
'''

##### Discover services

'''javascript
peripheral.discoverServices(); // any service UUID
...
```

#### <a name="apidoc.element.noble.noble.prototype.write"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>write (peripheralUuid, serviceUuid, characteristicUuid, data, withoutResponse)](#apidoc.element.noble.noble.prototype.write)
- description and source-code
```javascript
write = function (peripheralUuid, serviceUuid, characteristicUuid, data, withoutResponse) {
   this._bindings.write(peripheralUuid, serviceUuid, characteristicUuid, data, withoutResponse);
}
```
- example usage
```shell
...
'''javascript
characteristic.read([callback(error, data)]);
'''

##### Write

'''javascript
characteristic.write(data, withoutResponse[, callback(error)]); // data is a buffer, withoutResponse is true|false
'''

* '''withoutResponse''':
  * '''false''': send a write request, used with "write" characteristic property
  * '''true''': send a write command, used with "write without response" characteristic property

##### Broadcast
...
```

#### <a name="apidoc.element.noble.noble.prototype.writeHandle"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>writeHandle (peripheralUuid, handle, data, withoutResponse)](#apidoc.element.noble.noble.prototype.writeHandle)
- description and source-code
```javascript
writeHandle = function (peripheralUuid, handle, data, withoutResponse) {
  this._bindings.writeHandle(peripheralUuid, handle, data, withoutResponse);
}
```
- example usage
```shell
...
'''javascript
peripheral.readHandle(handle, callback(error, data));
'''

##### Write

'''javascript
peripheral.writeHandle(handle, data, withoutResponse, callback(error));
'''

### Events

See [Node.js EventEmitter docs](https://nodejs.org/api/events.html) for more info. on API's.

#### Adapter state change
...
```

#### <a name="apidoc.element.noble.noble.prototype.writeValue"></a>[function <span class="apidocSignatureSpan">noble.noble.prototype.</span>writeValue (peripheralUuid, serviceUuid, characteristicUuid, descriptorUuid, data)](#apidoc.element.noble.noble.prototype.writeValue)
- description and source-code
```javascript
writeValue = function (peripheralUuid, serviceUuid, characteristicUuid, descriptorUuid, data) {
  this._bindings.writeValue(peripheralUuid, serviceUuid, characteristicUuid, descriptorUuid, data);
}
```
- example usage
```shell
...
'''javascript
descriptor.readValue([callback(error, data)]);
'''

##### Write value

'''javascript
descriptor.writeValue(data[, callback(error)]); // data is a buffer
'''

#### Handle

##### Read

'''javascript
...
```



# <a name="apidoc.module.noble.peripheral"></a>[module noble.peripheral](#apidoc.module.noble.peripheral)

#### <a name="apidoc.element.noble.peripheral.peripheral"></a>[function <span class="apidocSignatureSpan">noble.</span>peripheral (noble, id, address, addressType, connectable, advertisement, rssi)](#apidoc.element.noble.peripheral.peripheral)
- description and source-code
```javascript
function Peripheral(noble, id, address, addressType, connectable, advertisement, rssi) {
  this._noble = noble;

  this.id = id;
  this.uuid = id; // for legacy
  this.address = address;
  this.addressType = addressType;
  this.connectable = connectable;
  this.advertisement = advertisement;
  this.rssi = rssi;
  this.services = null;
  this.state = 'disconnected';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.peripheral.super_"></a>[function <span class="apidocSignatureSpan">noble.peripheral.</span>super_ ()](#apidoc.element.noble.peripheral.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.noble.peripheral.prototype"></a>[module noble.peripheral.prototype](#apidoc.module.noble.peripheral.prototype)

#### <a name="apidoc.element.noble.peripheral.prototype.connect"></a>[function <span class="apidocSignatureSpan">noble.peripheral.prototype.</span>connect (callback)](#apidoc.element.noble.peripheral.prototype.connect)
- description and source-code
```javascript
connect = function (callback) {
  if (callback) {
    this.once('connect', function(error) {
      callback(error);
    });
  }

  if (this.state === 'connected') {
    this.emit('connect', new Error('Peripheral already connected'));
  } else {
    this.state = 'connecting';
    this._noble.connect(this.id);
  }
}
```
- example usage
```shell
...
'''

#### Peripheral

##### Connect

'''javascript
peripheral.connect([callback(error)]);
'''

##### Disconnect or cancel pending connection

'''javascript
peripheral.disconnect([callback(error)]);
'''
...
```

#### <a name="apidoc.element.noble.peripheral.prototype.disconnect"></a>[function <span class="apidocSignatureSpan">noble.peripheral.prototype.</span>disconnect (callback)](#apidoc.element.noble.peripheral.prototype.disconnect)
- description and source-code
```javascript
disconnect = function (callback) {
  if (callback) {
    this.once('disconnect', function() {
      callback(null);
    });
  }
  this.state = 'disconnecting';
  this._noble.disconnect(this.id);
}
```
- example usage
```shell
...
'''javascript
peripheral.connect([callback(error)]);
'''

##### Disconnect or cancel pending connection

'''javascript
peripheral.disconnect([callback(error)]);
'''

##### Update RSSI

'''javascript
peripheral.updateRssi([callback(error, rssi)]);
'''
...
```

#### <a name="apidoc.element.noble.peripheral.prototype.discoverAllServicesAndCharacteristics"></a>[function <span class="apidocSignatureSpan">noble.peripheral.prototype.</span>discoverAllServicesAndCharacteristics (callback)](#apidoc.element.noble.peripheral.prototype.discoverAllServicesAndCharacteristics)
- description and source-code
```javascript
discoverAllServicesAndCharacteristics = function (callback) {
  this.discoverSomeServicesAndCharacteristics([], [], callback);
}
```
- example usage
```shell
...
var serviceUUIDs = ["<service UUID 1>", ...];
peripheral.discoverServices(serviceUUIDs[, callback(error, services)]); // particular UUID's
'''

##### Discover all services and characteristics

'''javascript
peripheral.discoverAllServicesAndCharacteristics([callback(error, services, characteristics));
'''

##### Discover some services and characteristics

'''javascript
var serviceUUIDs = ["<service UUID 1>", ...];
var characteristicUUIDs = ["<characteristic UUID 1>", ...];
...
```

#### <a name="apidoc.element.noble.peripheral.prototype.discoverServices"></a>[function <span class="apidocSignatureSpan">noble.peripheral.prototype.</span>discoverServices (uuids, callback)](#apidoc.element.noble.peripheral.prototype.discoverServices)
- description and source-code
```javascript
discoverServices = function (uuids, callback) {
  if (callback) {
    this.once('servicesDiscover', function(services) {
      callback(null, services);
    });
  }

  this._noble.discoverServices(this.id, uuids);
}
```
- example usage
```shell
...
'''javascript
peripheral.updateRssi([callback(error, rssi)]);
'''

##### Discover services

'''javascript
peripheral.discoverServices(); // any service UUID

var serviceUUIDs = ["<service UUID 1>", ...];
peripheral.discoverServices(serviceUUIDs[, callback(error, services)]); // particular UUID's
'''

##### Discover all services and characteristics
...
```

#### <a name="apidoc.element.noble.peripheral.prototype.discoverSomeServicesAndCharacteristics"></a>[function <span class="apidocSignatureSpan">noble.peripheral.prototype.</span>discoverSomeServicesAndCharacteristics (serviceUuids, characteristicsUuids, callback)](#apidoc.element.noble.peripheral.prototype.discoverSomeServicesAndCharacteristics)
- description and source-code
```javascript
discoverSomeServicesAndCharacteristics = function (serviceUuids, characteristicsUuids, callback) {
  this.discoverServices(serviceUuids, function(err, services) {
    var numDiscovered = 0;
    var allCharacteristics = [];

    for (var i in services) {
      var service = services[i];

      service.discoverCharacteristics(characteristicsUuids, function(error, characteristics) {
        numDiscovered++;

        if (error === null) {
          for (var j in characteristics) {
            var characteristic = characteristics[j];

            allCharacteristics.push(characteristic);
          }
        }

        if (numDiscovered === services.length) {
          if (callback) {
            callback(null, services, allCharacteristics);
          }
        }
      }.bind(this));
    }
  }.bind(this));
}
```
- example usage
```shell
...
'''

##### Discover some services and characteristics

'''javascript
var serviceUUIDs = ["<service UUID 1>", ...];
var characteristicUUIDs = ["<characteristic UUID 1>", ...];
peripheral.discoverSomeServicesAndCharacteristics(serviceUUIDs, characteristicUUIDs, [callback(error, services, characteristics));
'''
#### Service

##### Discover included services

'''javascript
service.discoverIncludedServices(); // any service UUID
...
```

#### <a name="apidoc.element.noble.peripheral.prototype.readHandle"></a>[function <span class="apidocSignatureSpan">noble.peripheral.prototype.</span>readHandle (handle, callback)](#apidoc.element.noble.peripheral.prototype.readHandle)
- description and source-code
```javascript
readHandle = function (handle, callback) {
  if (callback) {
    this.once('handleRead' + handle, function(data) {
      callback(null, data);
    });
  }

  this._noble.readHandle(this.id, handle);
}
```
- example usage
```shell
...
'''

#### Handle

##### Read

'''javascript
peripheral.readHandle(handle, callback(error, data));
'''

##### Write

'''javascript
peripheral.writeHandle(handle, data, withoutResponse, callback(error));
'''
...
```

#### <a name="apidoc.element.noble.peripheral.prototype.toString"></a>[function <span class="apidocSignatureSpan">noble.peripheral.prototype.</span>toString ()](#apidoc.element.noble.peripheral.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return JSON.stringify({
    id: this.id,
    address: this.address,
    addressType: this.addressType,
    connectable: this.connectable,
    advertisement: this.advertisement,
    rssi: this.rssi,
    state: this.state
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.peripheral.prototype.updateRssi"></a>[function <span class="apidocSignatureSpan">noble.peripheral.prototype.</span>updateRssi (callback)](#apidoc.element.noble.peripheral.prototype.updateRssi)
- description and source-code
```javascript
updateRssi = function (callback) {
  if (callback) {
    this.once('rssiUpdate', function(rssi) {
      callback(null, rssi);
    });
  }

  this._noble.updateRssi(this.id);
}
```
- example usage
```shell
...
'''javascript
peripheral.disconnect([callback(error)]);
'''

##### Update RSSI

'''javascript
peripheral.updateRssi([callback(error, rssi)]);
'''

##### Discover services

'''javascript
peripheral.discoverServices(); // any service UUID
...
```

#### <a name="apidoc.element.noble.peripheral.prototype.writeHandle"></a>[function <span class="apidocSignatureSpan">noble.peripheral.prototype.</span>writeHandle (handle, data, withoutResponse, callback)](#apidoc.element.noble.peripheral.prototype.writeHandle)
- description and source-code
```javascript
writeHandle = function (handle, data, withoutResponse, callback) {
  if (!(data instanceof Buffer)) {
    throw new Error('data must be a Buffer');
  }

  if (callback) {
    this.once('handleWrite' + handle, function() {
      callback(null);
    });
  }

  this._noble.writeHandle(this.id, handle, data, withoutResponse);
}
```
- example usage
```shell
...
'''javascript
peripheral.readHandle(handle, callback(error, data));
'''

##### Write

'''javascript
peripheral.writeHandle(handle, data, withoutResponse, callback(error));
'''

### Events

See [Node.js EventEmitter docs](https://nodejs.org/api/events.html) for more info. on API's.

#### Adapter state change
...
```



# <a name="apidoc.module.noble.service"></a>[module noble.service](#apidoc.module.noble.service)

#### <a name="apidoc.element.noble.service.service"></a>[function <span class="apidocSignatureSpan">noble.</span>service (noble, peripheralId, uuid)](#apidoc.element.noble.service.service)
- description and source-code
```javascript
function Service(noble, peripheralId, uuid) {
  this._noble = noble;
  this._peripheralId = peripheralId;

  this.uuid = uuid;
  this.name = null;
  this.type = null;
  this.includedServiceUuids = null;
  this.characteristics = null;

  var service = services[uuid];
  if (service) {
    this.name = service.name;
    this.type = service.type;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.noble.service.super_"></a>[function <span class="apidocSignatureSpan">noble.service.</span>super_ ()](#apidoc.element.noble.service.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.noble.service.prototype"></a>[module noble.service.prototype](#apidoc.module.noble.service.prototype)

#### <a name="apidoc.element.noble.service.prototype.discoverCharacteristics"></a>[function <span class="apidocSignatureSpan">noble.service.prototype.</span>discoverCharacteristics (characteristicUuids, callback)](#apidoc.element.noble.service.prototype.discoverCharacteristics)
- description and source-code
```javascript
discoverCharacteristics = function (characteristicUuids, callback) {
  if (callback) {
    this.once('characteristicsDiscover', function(characteristics) {
      callback(null, characteristics);
    });
  }

  this._noble.discoverCharacteristics(
    this._peripheralId,
    this.uuid,
    characteristicUuids
  );
}
```
- example usage
```shell
...
var serviceUUIDs = ["<service UUID 1>", ...];
service.discoverIncludedServices(serviceUUIDs[, callback(error, includedServiceUuids)]); // particular UUID's
'''

##### Discover characteristics

'''javascript
service.discoverCharacteristics() // any characteristic UUID

var characteristicUUIDs = ["<characteristic UUID 1>", ...];
service.discoverCharacteristics(characteristicUUIDs[, callback(error, characteristics)]); // particular UUID's
'''

#### Characteristic
...
```

#### <a name="apidoc.element.noble.service.prototype.discoverIncludedServices"></a>[function <span class="apidocSignatureSpan">noble.service.prototype.</span>discoverIncludedServices (serviceUuids, callback)](#apidoc.element.noble.service.prototype.discoverIncludedServices)
- description and source-code
```javascript
discoverIncludedServices = function (serviceUuids, callback) {
  if (callback) {
    this.once('includedServicesDiscover', function(includedServiceUuids) {
      callback(null, includedServiceUuids);
    });
  }

  this._noble.discoverIncludedServices(
    this._peripheralId,
    this.uuid,
    serviceUuids
  );
}
```
- example usage
```shell
...
peripheral.discoverSomeServicesAndCharacteristics(serviceUUIDs, characteristicUUIDs, [callback(error, services, characteristics));
'''
#### Service

##### Discover included services

'''javascript
service.discoverIncludedServices(); // any service UUID

var serviceUUIDs = ["<service UUID 1>", ...];
service.discoverIncludedServices(serviceUUIDs[, callback(error, includedServiceUuids)]); // particular UUID's
'''

##### Discover characteristics
...
```

#### <a name="apidoc.element.noble.service.prototype.toString"></a>[function <span class="apidocSignatureSpan">noble.service.prototype.</span>toString ()](#apidoc.element.noble.service.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return JSON.stringify({
    uuid: this.uuid,
    name: this.name,
    type: this.type,
    includedServiceUuids: this.includedServiceUuids
  });
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
