<!--
    SPDX-FileCopyrightText: Copyright (C) swift Project Community / Contributors
    SPDX-License-Identifier: GFDL-1.3-only
-->

This document covers some technical details for matching script programmers

## Matching script interacting with swift

There are classes, which may be used as objects in Matching script (i.e. JavaScript).
Those classes start with a `MS` prefix (matching script).
Those classes can be found in `BlackMisc::Simulation` and `BlackCore`.

- MSInOutValues
- MSModelSet
- MSWebServices

## Using properties


MS class properties as below

```cpp
//! MSNetworkValues properties @{
Q_PROPERTY(QString callsign           READ getCallsign           WRITE setCallsign           NOTIFY callsignChanged)
Q_PROPERTY(QString callsignAsSet      READ getCallsignAsSet)
Q_PROPERTY(QString flightNumber       READ getFlightNumber)
Q_PROPERTY(int     dbAircraftIcaoId   READ getDbAircraftIcaoId   WRITE setDbAircraftIcaoId   NOTIFY
```

can be used in matching script as follows

```js
outObject.aircraftIcao = "C172";
outObject.modified     = true; // tell we changed something
```

Some properties are read only, and you can see the type from property definition.

## Using functions

Functions of MS classes can be used if they are marked as `Q_INVOKABLE` (only those you can invoke from matching script).

```cpp
//! Functions calling the web services @{
Q_INVOKABLE int countAircraftIcaoCodesForDesignator(const QString &designator) const;
Q_INVOKABLE int countAirlineIcaoCodesForDesignator(const QString &designator) const;
//! @}
```

or

```cpp
//! Model string of model with closest color distance
Q_INVOKABLE QString findCombinedTypeWithClosestColorLivery(const QString &combinedType, const QString &rgbColor) const;
```

Those you can call those as functions in matching script

```js
var mscl = modelSet.findCombinedTypeWithClosestColorLivery(combinedType, white);
```

## Examples


Check out the `matchingscript` directory for examples, like `\swift-0.9.2-64bit\share\matchingscript`.
