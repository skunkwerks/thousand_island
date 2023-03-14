# Changelog for 0.6.x

## 0.6.2 (22 Feb 2023)

### Fixes

* Fixes a race condition at application shutdown that caused spurious acceptor
  crashes to litter the logs (#44). Thanks @danschultzer!


## 0.6.1 (19 Feb 2023)

### Changes

* Expose ThousandIsland.Telemetry.t() as a transparent type
* Pass telemetry errors in metadata rather than metrics
* Allow explicit passing of start times into telemetry spans

## 0.6.0 (4 Feb 2023)

### Enhancements

* (Re)introduce telemetry support as specified in the `ThousandIsland.Telemetry`
  module

# Changelog for 0.5.x

## 0.5.17 (31 Jan 2023)

### Enhancements

* Add `ThousandIsland.connection_pids/1` to enumerate connection processes

## 0.5.16 (21 Jan 2023)

### Enhancements

* Narrow internal pattern matches to enable Handlers to use their own socket calls (#39)

### Fixes

* Fix documentation typos

## 0.5.15 (10 Jan 2023)

### Enhancements

* Do not emit GenServer crash logs in connection timeout situations
* Doc updates