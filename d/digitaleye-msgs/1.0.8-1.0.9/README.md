# Comparing `tmp/digitaleye_msgs-1.0.8.tar.gz` & `tmp/digitaleye_msgs-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitaleye_msgs-1.0.8.tar", last modified: Sun Mar 24 18:38:21 2024, max compression
+gzip compressed data, was "digitaleye_msgs-1.0.9.tar", last modified: Thu May 23 11:24:28 2024, max compression
```

## Comparing `digitaleye_msgs-1.0.8.tar` & `digitaleye_msgs-1.0.9.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 18:38:21.923121 digitaleye_msgs-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      372 2024-03-24 18:38:21.923121 digitaleye_msgs-1.0.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 18:38:21.915120 digitaleye_msgs-1.0.8/digitaleye_msgs/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 18:38:21.923121 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/
--rw-r--r--   0 root         (0) root         (0)     5784 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_AccessSchedule.py
--rw-r--r--   0 root         (0) root         (0)     7300 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Action.py
--rw-r--r--   0 root         (0) root         (0)     4252 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_ActionStatus.py
--rw-r--r--   0 root         (0) root         (0)    14332 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Allocation.py
--rw-r--r--   0 root         (0) root         (0)     7248 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_AllocationTemplate.py
--rw-r--r--   0 root         (0) root         (0)     8760 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Booking.py
--rw-r--r--   0 root         (0) root         (0)     7543 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_BookingActions.py
--rw-r--r--   0 root         (0) root         (0)    15797 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_BookingAllocations.py
--rw-r--r--   0 root         (0) root         (0)     5194 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_BookingStatus.py
--rw-r--r--   0 root         (0) root         (0)     5447 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Breach.py
--rw-r--r--   0 root         (0) root         (0)     6039 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_BreachPicture.py
--rw-r--r--   0 root         (0) root         (0)    32535 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_ComponentState.py
--rw-r--r--   0 root         (0) root         (0)     8333 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Conformance.py
--rw-r--r--   0 root         (0) root         (0)     8508 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_ConformanceStatus.py
--rw-r--r--   0 root         (0) root         (0)     4649 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_ConformanceUavStatus.py
--rw-r--r--   0 root         (0) root         (0)    25598 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Constants.py
--rw-r--r--   0 root         (0) root         (0)     3766 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_ConstantsAllocations.py
--rw-r--r--   0 root         (0) root         (0)     3606 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_ConstantsBookings.py
--rw-r--r--   0 root         (0) root         (0)     3852 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_ConstantsConformance.py
--rw-r--r--   0 root         (0) root         (0)    46686 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_DigitalEyeStatus.py
--rw-r--r--   0 root         (0) root         (0)     6347 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Flightpath.py
--rw-r--r--   0 root         (0) root         (0)     4562 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Flightpoint.py
--rw-r--r--   0 root         (0) root         (0)     4981 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_GNSSPosition.py
--rw-r--r--   0 root         (0) root         (0)     5967 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_GNSSState.py
--rw-r--r--   0 root         (0) root         (0)    15312 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_IMUValue.py
--rw-r--r--   0 root         (0) root         (0)     6024 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_MASDefinition.py
--rw-r--r--   0 root         (0) root         (0)    12015 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_MGSDefinition.py
--rw-r--r--   0 root         (0) root         (0)     7715 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_MGSStatus.py
--rw-r--r--   0 root         (0) root         (0)     9048 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_MVSControl.py
--rw-r--r--   0 root         (0) root         (0)     5290 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Metric.py
--rw-r--r--   0 root         (0) root         (0)    32685 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Object.py
--rw-r--r--   0 root         (0) root         (0)    35359 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_ObjectList.py
--rw-r--r--   0 root         (0) root         (0)     4165 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Pause.py
--rw-r--r--   0 root         (0) root         (0)    41510 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Pole.py
--rw-r--r--   0 root         (0) root         (0)    17362 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_PolePose.py
--rw-r--r--   0 root         (0) root         (0)    43006 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Position.py
--rw-r--r--   0 root         (0) root         (0)     6869 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Sector.py
--rw-r--r--   0 root         (0) root         (0)     7681 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_SectorPicture.py
--rw-r--r--   0 root         (0) root         (0)    26501 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Sensor.py
--rw-r--r--   0 root         (0) root         (0)     7414 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_SensorPose.py
--rw-r--r--   0 root         (0) root         (0)     9187 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_State.py
--rw-r--r--   0 root         (0) root         (0)     7406 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_SystemCommand.py
--rw-r--r--   0 root         (0) root         (0)    29661 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_SystemConfiguration.py
--rw-r--r--   0 root         (0) root         (0)     6955 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_SystemNotification.py
--rw-r--r--   0 root         (0) root         (0)    39127 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_SystemState.py
--rw-r--r--   0 root         (0) root         (0)     4270 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_SystemTransition.py
--rw-r--r--   0 root         (0) root         (0)     4232 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_TimeSlot.py
--rw-r--r--   0 root         (0) root         (0)    11241 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_UavExtReport.py
--rw-r--r--   0 root         (0) root         (0)    13838 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_UavExtReportList.py
--rw-r--r--   0 root         (0) root         (0)    11464 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_UavFlightData.py
--rw-r--r--   0 root         (0) root         (0)     6825 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_UavGeneralMsg.py
--rw-r--r--   0 root         (0) root         (0)    13137 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_UavIntReport.py
--rw-r--r--   0 root         (0) root         (0)    16594 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_UavIntReportList.py
--rw-r--r--   0 root         (0) root         (0)     6760 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_UavState.py
--rw-r--r--   0 root         (0) root         (0)     9854 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_UavStateList.py
--rw-r--r--   0 root         (0) root         (0)     8197 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_VehicleCommand.py
--rw-r--r--   0 root         (0) root         (0)     6206 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Volume.py
--rw-r--r--   0 root         (0) root         (0)     6668 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Zone.py
--rw-r--r--   0 root         (0) root         (0)     5575 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_ZoneObjectStatus.py
--rw-r--r--   0 root         (0) root         (0)     1687 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/msg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 18:38:21.923121 digitaleye_msgs-1.0.8/digitaleye_msgs/srv/
--rw-r--r--   0 root         (0) root         (0)     9294 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_BookingUpdate.py
--rw-r--r--   0 root         (0) root         (0)     8752 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_GetBookingStatus.py
--rw-r--r--   0 root         (0) root         (0)     9332 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_GetBookings.py
--rw-r--r--   0 root         (0) root         (0)    16261 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_GetEntrypoint.py
--rw-r--r--   0 root         (0) root         (0)    11299 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_GetFlightpath.py
--rw-r--r--   0 root         (0) root         (0)    38914 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_GetMGSObjects.py
--rw-r--r--   0 root         (0) root         (0)    11294 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_GetMGSStatus.py
--rw-r--r--   0 root         (0) root         (0)    11387 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_GetNotifications.py
--rw-r--r--   0 root         (0) root         (0)    46707 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_GetPoles.py
--rw-r--r--   0 root         (0) root         (0)    10761 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_GetSchedule.py
--rw-r--r--   0 root         (0) root         (0)    50091 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_GetStatus.py
--rw-r--r--   0 root         (0) root         (0)    17472 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_GetUAVExternalReport.py
--rw-r--r--   0 root         (0) root         (0)    20187 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_GetUAVInternalReport.py
--rw-r--r--   0 root         (0) root         (0)     8517 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_GetUavIdInt.py
--rw-r--r--   0 root         (0) root         (0)     8564 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_GetUavIdString.py
--rw-r--r--   0 root         (0) root         (0)    13553 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_NewBooking.py
--rw-r--r--   0 root         (0) root         (0)    10461 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_PointConversion.py
--rw-r--r--   0 root         (0) root         (0)      514 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs/srv/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-24 18:38:21.923121 digitaleye_msgs-1.0.8/digitaleye_msgs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      372 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3223 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/digitaleye_msgs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-24 18:38:21.923121 digitaleye_msgs-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      497 2024-03-24 18:38:21.000000 digitaleye_msgs-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:24:28.848030 digitaleye_msgs-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      372 2024-05-23 11:24:28.848030 digitaleye_msgs-1.0.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:24:28.836030 digitaleye_msgs-1.0.9/digitaleye_msgs/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:24:28.844030 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/
+-rw-r--r--   0 root         (0) root         (0)     5784 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_AccessSchedule.py
+-rw-r--r--   0 root         (0) root         (0)     7300 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Action.py
+-rw-r--r--   0 root         (0) root         (0)     4252 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_ActionStatus.py
+-rw-r--r--   0 root         (0) root         (0)    14332 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Allocation.py
+-rw-r--r--   0 root         (0) root         (0)     7248 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_AllocationTemplate.py
+-rw-r--r--   0 root         (0) root         (0)     8760 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Booking.py
+-rw-r--r--   0 root         (0) root         (0)     7543 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_BookingActions.py
+-rw-r--r--   0 root         (0) root         (0)    15797 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_BookingAllocations.py
+-rw-r--r--   0 root         (0) root         (0)     5194 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_BookingStatus.py
+-rw-r--r--   0 root         (0) root         (0)     5447 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Breach.py
+-rw-r--r--   0 root         (0) root         (0)     6039 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_BreachPicture.py
+-rw-r--r--   0 root         (0) root         (0)    32535 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_ComponentState.py
+-rw-r--r--   0 root         (0) root         (0)     8333 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Conformance.py
+-rw-r--r--   0 root         (0) root         (0)     8508 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_ConformanceStatus.py
+-rw-r--r--   0 root         (0) root         (0)     4649 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_ConformanceUavStatus.py
+-rw-r--r--   0 root         (0) root         (0)    25598 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Constants.py
+-rw-r--r--   0 root         (0) root         (0)     3766 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_ConstantsAllocations.py
+-rw-r--r--   0 root         (0) root         (0)     3606 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_ConstantsBookings.py
+-rw-r--r--   0 root         (0) root         (0)     3852 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_ConstantsConformance.py
+-rw-r--r--   0 root         (0) root         (0)    46686 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_DigitalEyeStatus.py
+-rw-r--r--   0 root         (0) root         (0)     6347 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Flightpath.py
+-rw-r--r--   0 root         (0) root         (0)     4562 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Flightpoint.py
+-rw-r--r--   0 root         (0) root         (0)     4981 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_GNSSPosition.py
+-rw-r--r--   0 root         (0) root         (0)     5967 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_GNSSState.py
+-rw-r--r--   0 root         (0) root         (0)    15312 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_IMUValue.py
+-rw-r--r--   0 root         (0) root         (0)     6024 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_MASDefinition.py
+-rw-r--r--   0 root         (0) root         (0)    12015 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_MGSDefinition.py
+-rw-r--r--   0 root         (0) root         (0)     7715 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_MGSStatus.py
+-rw-r--r--   0 root         (0) root         (0)     9048 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_MVSControl.py
+-rw-r--r--   0 root         (0) root         (0)     5290 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Metric.py
+-rw-r--r--   0 root         (0) root         (0)    19109 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Object.py
+-rw-r--r--   0 root         (0) root         (0)    21532 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_ObjectList.py
+-rw-r--r--   0 root         (0) root         (0)     4165 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Pause.py
+-rw-r--r--   0 root         (0) root         (0)    41510 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Pole.py
+-rw-r--r--   0 root         (0) root         (0)    17362 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_PolePose.py
+-rw-r--r--   0 root         (0) root         (0)    43006 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Position.py
+-rw-r--r--   0 root         (0) root         (0)     6869 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Sector.py
+-rw-r--r--   0 root         (0) root         (0)     7681 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_SectorPicture.py
+-rw-r--r--   0 root         (0) root         (0)    26501 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Sensor.py
+-rw-r--r--   0 root         (0) root         (0)     7414 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_SensorPose.py
+-rw-r--r--   0 root         (0) root         (0)     9187 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_State.py
+-rw-r--r--   0 root         (0) root         (0)     7406 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_SystemCommand.py
+-rw-r--r--   0 root         (0) root         (0)    29661 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_SystemConfiguration.py
+-rw-r--r--   0 root         (0) root         (0)     6955 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_SystemNotification.py
+-rw-r--r--   0 root         (0) root         (0)    39127 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_SystemState.py
+-rw-r--r--   0 root         (0) root         (0)     4270 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_SystemTransition.py
+-rw-r--r--   0 root         (0) root         (0)     4232 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_TimeSlot.py
+-rw-r--r--   0 root         (0) root         (0)    11241 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_UavExtReport.py
+-rw-r--r--   0 root         (0) root         (0)    13838 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_UavExtReportList.py
+-rw-r--r--   0 root         (0) root         (0)    11464 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_UavFlightData.py
+-rw-r--r--   0 root         (0) root         (0)     6825 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_UavGeneralMsg.py
+-rw-r--r--   0 root         (0) root         (0)    13137 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_UavIntReport.py
+-rw-r--r--   0 root         (0) root         (0)    16594 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_UavIntReportList.py
+-rw-r--r--   0 root         (0) root         (0)     6760 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_UavState.py
+-rw-r--r--   0 root         (0) root         (0)     9854 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_UavStateList.py
+-rw-r--r--   0 root         (0) root         (0)     8197 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_VehicleCommand.py
+-rw-r--r--   0 root         (0) root         (0)     6206 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Volume.py
+-rw-r--r--   0 root         (0) root         (0)     6668 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Zone.py
+-rw-r--r--   0 root         (0) root         (0)     5575 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_ZoneObjectStatus.py
+-rw-r--r--   0 root         (0) root         (0)     1687 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/msg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:24:28.844030 digitaleye_msgs-1.0.9/digitaleye_msgs/srv/
+-rw-r--r--   0 root         (0) root         (0)     9294 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_BookingUpdate.py
+-rw-r--r--   0 root         (0) root         (0)     8752 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetBookingStatus.py
+-rw-r--r--   0 root         (0) root         (0)     9332 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetBookings.py
+-rw-r--r--   0 root         (0) root         (0)    16261 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetEntrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    11299 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetFlightpath.py
+-rw-r--r--   0 root         (0) root         (0)    25087 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetMGSObjects.py
+-rw-r--r--   0 root         (0) root         (0)    11294 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetMGSStatus.py
+-rw-r--r--   0 root         (0) root         (0)    11387 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetNotifications.py
+-rw-r--r--   0 root         (0) root         (0)    46707 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetPoles.py
+-rw-r--r--   0 root         (0) root         (0)    10761 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetSchedule.py
+-rw-r--r--   0 root         (0) root         (0)    50091 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetStatus.py
+-rw-r--r--   0 root         (0) root         (0)    17472 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetUAVExternalReport.py
+-rw-r--r--   0 root         (0) root         (0)    20187 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetUAVInternalReport.py
+-rw-r--r--   0 root         (0) root         (0)     8517 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetUavIdInt.py
+-rw-r--r--   0 root         (0) root         (0)     8564 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetUavIdString.py
+-rw-r--r--   0 root         (0) root         (0)    13553 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_NewBooking.py
+-rw-r--r--   0 root         (0) root         (0)    10461 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_PointConversion.py
+-rw-r--r--   0 root         (0) root         (0)      514 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs/srv/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:24:28.848030 digitaleye_msgs-1.0.9/digitaleye_msgs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      372 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3223 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/digitaleye_msgs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 11:24:28.848030 digitaleye_msgs-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      497 2024-05-23 11:24:28.000000 digitaleye_msgs-1.0.9/setup.py
```

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_AccessSchedule.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_AccessSchedule.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Action.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Action.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_ActionStatus.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_ActionStatus.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Allocation.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Allocation.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_AllocationTemplate.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_AllocationTemplate.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Booking.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Booking.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_BookingActions.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_BookingActions.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_BookingAllocations.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_BookingAllocations.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_BookingStatus.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_BookingStatus.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Breach.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Breach.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_BreachPicture.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_BreachPicture.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_ComponentState.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_ComponentState.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Conformance.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Conformance.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_ConformanceStatus.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_ConformanceStatus.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_ConformanceUavStatus.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_ConformanceUavStatus.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Constants.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Constants.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_ConstantsAllocations.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_ConstantsAllocations.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_ConstantsBookings.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_ConstantsBookings.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_ConstantsConformance.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_ConstantsConformance.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_DigitalEyeStatus.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_DigitalEyeStatus.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Flightpath.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Flightpath.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Flightpoint.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Flightpoint.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_GNSSPosition.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_GNSSPosition.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_GNSSState.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_GNSSState.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_IMUValue.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_IMUValue.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_MASDefinition.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_MASDefinition.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_MGSDefinition.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_MGSDefinition.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_MGSStatus.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_MGSStatus.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_MVSControl.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_MVSControl.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Metric.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Metric.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Object.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_SystemConfiguration.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,815 +1,897 @@
 # This Python file uses the following encoding: utf-8
-"""autogenerated by genpy from digitaleye_msgs/Object.msg. Do not edit."""
+"""autogenerated by genpy from digitaleye_msgs/SystemConfiguration.msg. Do not edit."""
 import codecs
 import sys
 python3 = True if sys.hexversion > 0x03000000 else False
 import genpy
 import struct
 
 import digitaleye_msgs.msg
-import genpy
 import geometry_msgs.msg
+import sensor_msgs.msg
 import std_msgs.msg
-import visualization_msgs.msg
 
-class Object(genpy.Message):
-  _md5sum = "50a51e88bc1d873cad22eaf4e5964098"
-  _type = "digitaleye_msgs/Object"
-  _has_header = True  # flag to mark the presence of a Header object
-  _full_text = """# Description of an object in the Monitored Space
+class SystemConfiguration(genpy.Message):
+  _md5sum = "aa0494b2170d4b3eac19f93e9fcd5c9c"
+  _type = "digitaleye_msgs/SystemConfiguration"
+  _has_header = False  # flag to mark the presence of a Header object
+  _full_text = """# Configuration of a DigitalEye subsystem
+
+# unique identifier of the configured subsystem
+uint32 system_id
+
+# subsystem’s network IP address
+string ip_address
+
+# port on which the subsystem is accepting
+# incoming connections from the DEMS
+uint32 port
+
+# list of monitoring sensor(s) attached to this subsystem
+digitaleye_msgs/Sensor[] sensors
+
+================================================================================
+MSG: digitaleye_msgs/Sensor
+# Description of a monitoring DigitalEye sensor
+# and its properties
 
-# information on the time at which the object
-# was reported (epoch time) and its reference frame
-std_msgs/Header header
+# unique identifier of the sensor
+# e.g. hardware serial number
+string sensor_id
 
-# id assigned to the reported object
-uint64 object_id
+# brand/model of sensor hardware
+string model
 
-# list of ID(s) of reported object(s) which
-# constitute it (if fused)
-uint64[] fused_ids
+# type of sensor being described
+# e.g. camera, LIDAR, etc.
+uint32 type
 
-# coordinates of the object’s estimated position
-# in the local reference frame (meters)
-geometry_msgs/Point position
+# position of the sensor in
+# the DigitalEye’s local reference frame (meters)
+geometry_msgs/Pose pose
 
-# 3D covariance of the object position, represents the quality
-# of the position estimate, higher covariances mean
-# a worse estimate. XX, XY, XZ, YX, YY, YZ, ZX, ZY, ZZ
-float32[9] pos_covariance
+# direction in which the sensor is facing
+# with respect to the local frame’s x-axis
+float32 azimuth
 
-# estimated accuracy radius of object's position (meters)
-float32 accuracy
+# resolution height of the image captured by the sensor
+uint32 image_width
 
-# estimated velocity of the object (m/s)
-geometry_msgs/Vector3 velocity
+# resolution width of the image captured by the sensor
+uint32 image_height
 
-# estimated acceleration of the object (m/s2)
-geometry_msgs/Accel acceleration
+# frame rate of a vision sensor
+uint32 frame_rate
 
-# estimated size of the object (meters)
-float32 size
+# sensor’s current power level
+float32 power
 
-# object’s category
-# e.g. Personnel, Package, Passenger, UAV, etc.
-string classification
+# Whether or not the sensor has been calibrated
+bool calibrated
 
-# list of zone(s) in which the object is
-ZoneObjectStatus[] zones
+# current state of the sensor
+digitaleye_msgs/State state
 
-# Object visualisation marker
-visualization_msgs/Marker bounding_cylinder
+# Sensor inertial measurements
+digitaleye_msgs/IMUValue imu
 
 ================================================================================
-MSG: std_msgs/Header
-# Standard metadata for higher-level stamped data types.
-# This is generally used to communicate timestamped data 
-# in a particular coordinate frame.
-# 
-# sequence ID: consecutively increasing ID 
-uint32 seq
-#Two-integer timestamp that is expressed as:
-# * stamp.sec: seconds (stamp_secs) since epoch (in Python the variable is called 'secs')
-# * stamp.nsec: nanoseconds since stamp_secs (in Python the variable is called 'nsecs')
-# time-handling sugar is provided by the client library
-time stamp
-#Frame this data is associated with
-string frame_id
+MSG: geometry_msgs/Pose
+# A representation of pose in free space, composed of position and orientation. 
+Point position
+Quaternion orientation
 
 ================================================================================
 MSG: geometry_msgs/Point
 # This contains the position of a point in free space
 float64 x
 float64 y
 float64 z
 
 ================================================================================
-MSG: geometry_msgs/Vector3
-# This represents a vector in free space. 
-# It is only meant to represent a direction. Therefore, it does not
-# make sense to apply a translation to it (e.g., when applying a 
-# generic rigid transformation to a Vector3, tf2 will only apply the
-# rotation). If you want your data to be translatable too, use the
-# geometry_msgs/Point message instead.
+MSG: geometry_msgs/Quaternion
+# This represents an orientation in free space in quaternion form.
 
 float64 x
 float64 y
 float64 z
+float64 w
+
+================================================================================
+MSG: digitaleye_msgs/State
+# Details of a system’s status
+
+# unique identifier of the system
+# whose status is being reported
+uint32 id
+
+# system’s current state within the 
+# DigitalEye state machine
+uint32 state
+
+# system’s substatus within the current state,
+# unique to each system
+uint32 status
+
+# description of the system’s current state/status
+string description
+
+# timestamp indicating last change in state or status
+# (epoch time in sec)
+uint32 lastChange
+
+# list of performance metrics associated with the
+# current state
+digitaleye_msgs/Metric[] metrics
+
 ================================================================================
-MSG: geometry_msgs/Accel
-# This expresses acceleration in free space broken into its linear and angular parts.
-Vector3  linear
-Vector3  angular
+MSG: digitaleye_msgs/Metric
+# Performance indicator for a subsystem,
+# component or sensor
+
+# name of the performance indicator
+string name
+
+# value of the performance indicator
+string value
 
 ================================================================================
-MSG: digitaleye_msgs/ZoneObjectStatus
-# Status of the object within the specified zone
+MSG: digitaleye_msgs/IMUValue
+# Description of an IMU value reading
+
+# Imu heading
+float32 heading
+
+# Unique identifier of the sensor
+# e.g. hardware serial number
+string device_id
+
+# Imu measurements
+sensor_msgs/Imu imu
 
-# identifier of the zone the object is in
-uint32 zone_id
+# Magenetometer readings
+geometry_msgs/Vector3 magnetic_field
 
-# whether or not the object is allowed in the zone
-bool allowed
+# Imu reading of roll
+float32 roll
 
-# time the object was first detected in this zone
-# (ros timestamp in epoch time)
-time first_detected
-
-# time the object was last detected in this zone
-# (ros timestamp in epoch time)
-time last_detected
+# Imu reading of pitch
+float32 pitch
+
+# Calibration status
+bool deviceCalibrated
 
 ================================================================================
-MSG: visualization_msgs/Marker
-# See http://www.ros.org/wiki/rviz/DisplayTypes/Marker and http://www.ros.org/wiki/rviz/Tutorials/Markers%3A%20Basic%20Shapes for more information on using this message with rviz
+MSG: sensor_msgs/Imu
+# This is a message to hold data from an IMU (Inertial Measurement Unit)
+#
+# Accelerations should be in m/s^2 (not in g's), and rotational velocity should be in rad/sec
+#
+# If the covariance of the measurement is known, it should be filled in (if all you know is the 
+# variance of each measurement, e.g. from the datasheet, just put those along the diagonal)
+# A covariance matrix of all zeros will be interpreted as "covariance unknown", and to use the
+# data a covariance will have to be assumed or gotten from some other source
+#
+# If you have no estimate for one of the data elements (e.g. your IMU doesn't produce an orientation 
+# estimate), please set element 0 of the associated covariance matrix to -1
+# If you are interpreting this message, please check for a value of -1 in the first element of each 
+# covariance matrix, and disregard the associated estimate.
+
+Header header
+
+geometry_msgs/Quaternion orientation
+float64[9] orientation_covariance # Row major about x, y, z axes
+
+geometry_msgs/Vector3 angular_velocity
+float64[9] angular_velocity_covariance # Row major about x, y, z axes
 
-uint8 ARROW=0
-uint8 CUBE=1
-uint8 SPHERE=2
-uint8 CYLINDER=3
-uint8 LINE_STRIP=4
-uint8 LINE_LIST=5
-uint8 CUBE_LIST=6
-uint8 SPHERE_LIST=7
-uint8 POINTS=8
-uint8 TEXT_VIEW_FACING=9
-uint8 MESH_RESOURCE=10
-uint8 TRIANGLE_LIST=11
-
-uint8 ADD=0
-uint8 MODIFY=0
-uint8 DELETE=2
-uint8 DELETEALL=3
-
-Header header                        # header for time/frame information
-string ns                            # Namespace to place this object in... used in conjunction with id to create a unique name for the object
-int32 id 		                         # object ID useful in conjunction with the namespace for manipulating and deleting the object later
-int32 type 		                       # Type of object
-int32 action 	                       # 0 add/modify an object, 1 (deprecated), 2 deletes an object, 3 deletes all objects
-geometry_msgs/Pose pose                 # Pose of the object
-geometry_msgs/Vector3 scale             # Scale of the object 1,1,1 means default (usually 1 meter square)
-std_msgs/ColorRGBA color             # Color [0.0-1.0]
-duration lifetime                    # How long the object should last before being automatically deleted.  0 means forever
-bool frame_locked                    # If this marker should be frame-locked, i.e. retransformed into its frame every timestep
-
-#Only used if the type specified has some use for them (eg. POINTS, LINE_STRIP, ...)
-geometry_msgs/Point[] points
-#Only used if the type specified has some use for them (eg. POINTS, LINE_STRIP, ...)
-#number of colors must either be 0 or equal to the number of points
-#NOTE: alpha is not yet used
-std_msgs/ColorRGBA[] colors
-
-# NOTE: only used for text markers
-string text
-
-# NOTE: only used for MESH_RESOURCE markers
-string mesh_resource
-bool mesh_use_embedded_materials
+geometry_msgs/Vector3 linear_acceleration
+float64[9] linear_acceleration_covariance # Row major x, y z 
 
 ================================================================================
-MSG: geometry_msgs/Pose
-# A representation of pose in free space, composed of position and orientation. 
-Point position
-Quaternion orientation
+MSG: std_msgs/Header
+# Standard metadata for higher-level stamped data types.
+# This is generally used to communicate timestamped data 
+# in a particular coordinate frame.
+# 
+# sequence ID: consecutively increasing ID 
+uint32 seq
+#Two-integer timestamp that is expressed as:
+# * stamp.sec: seconds (stamp_secs) since epoch (in Python the variable is called 'secs')
+# * stamp.nsec: nanoseconds since stamp_secs (in Python the variable is called 'nsecs')
+# time-handling sugar is provided by the client library
+time stamp
+#Frame this data is associated with
+string frame_id
 
 ================================================================================
-MSG: geometry_msgs/Quaternion
-# This represents an orientation in free space in quaternion form.
+MSG: geometry_msgs/Vector3
+# This represents a vector in free space. 
+# It is only meant to represent a direction. Therefore, it does not
+# make sense to apply a translation to it (e.g., when applying a 
+# generic rigid transformation to a Vector3, tf2 will only apply the
+# rotation). If you want your data to be translatable too, use the
+# geometry_msgs/Point message instead.
 
 float64 x
 float64 y
-float64 z
-float64 w
-
-================================================================================
-MSG: std_msgs/ColorRGBA
-float32 r
-float32 g
-float32 b
-float32 a
-"""
-  __slots__ = ['header','object_id','fused_ids','position','pos_covariance','accuracy','velocity','acceleration','size','classification','zones','bounding_cylinder']
-  _slot_types = ['std_msgs/Header','uint64','uint64[]','geometry_msgs/Point','float32[9]','float32','geometry_msgs/Vector3','geometry_msgs/Accel','float32','string','digitaleye_msgs/ZoneObjectStatus[]','visualization_msgs/Marker']
+float64 z"""
+  __slots__ = ['system_id','ip_address','port','sensors']
+  _slot_types = ['uint32','string','uint32','digitaleye_msgs/Sensor[]']
 
   def __init__(self, *args, **kwds):
     """
     Constructor. Any message fields that are implicitly/explicitly
     set to None will be assigned a default value. The recommend
     use is keyword arguments as this is more robust to future message
     changes.  You cannot mix in-order arguments and keyword arguments.
 
     The available fields are:
-       header,object_id,fused_ids,position,pos_covariance,accuracy,velocity,acceleration,size,classification,zones,bounding_cylinder
+       system_id,ip_address,port,sensors
 
     :param args: complete set of field values, in .msg order
     :param kwds: use keyword arguments corresponding to message field names
     to set specific fields.
     """
     if args or kwds:
-      super(Object, self).__init__(*args, **kwds)
+      super(SystemConfiguration, self).__init__(*args, **kwds)
       # message fields cannot be None, assign default values for those that are
-      if self.header is None:
-        self.header = std_msgs.msg.Header()
-      if self.object_id is None:
-        self.object_id = 0
-      if self.fused_ids is None:
-        self.fused_ids = []
-      if self.position is None:
-        self.position = geometry_msgs.msg.Point()
-      if self.pos_covariance is None:
-        self.pos_covariance = [0.] * 9
-      if self.accuracy is None:
-        self.accuracy = 0.
-      if self.velocity is None:
-        self.velocity = geometry_msgs.msg.Vector3()
-      if self.acceleration is None:
-        self.acceleration = geometry_msgs.msg.Accel()
-      if self.size is None:
-        self.size = 0.
-      if self.classification is None:
-        self.classification = ''
-      if self.zones is None:
-        self.zones = []
-      if self.bounding_cylinder is None:
-        self.bounding_cylinder = visualization_msgs.msg.Marker()
+      if self.system_id is None:
+        self.system_id = 0
+      if self.ip_address is None:
+        self.ip_address = ''
+      if self.port is None:
+        self.port = 0
+      if self.sensors is None:
+        self.sensors = []
     else:
-      self.header = std_msgs.msg.Header()
-      self.object_id = 0
-      self.fused_ids = []
-      self.position = geometry_msgs.msg.Point()
-      self.pos_covariance = [0.] * 9
-      self.accuracy = 0.
-      self.velocity = geometry_msgs.msg.Vector3()
-      self.acceleration = geometry_msgs.msg.Accel()
-      self.size = 0.
-      self.classification = ''
-      self.zones = []
-      self.bounding_cylinder = visualization_msgs.msg.Marker()
+      self.system_id = 0
+      self.ip_address = ''
+      self.port = 0
+      self.sensors = []
 
   def _get_types(self):
     """
     internal API method
     """
     return self._slot_types
 
   def serialize(self, buff):
     """
     serialize message into buffer
     :param buff: buffer, ``StringIO``
     """
     try:
-      _x = self
-      buff.write(_get_struct_3I().pack(_x.header.seq, _x.header.stamp.secs, _x.header.stamp.nsecs))
-      _x = self.header.frame_id
+      _x = self.system_id
+      buff.write(_get_struct_I().pack(_x))
+      _x = self.ip_address
       length = len(_x)
       if python3 or type(_x) == unicode:
         _x = _x.encode('utf-8')
         length = len(_x)
       buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-      _x = self.object_id
-      buff.write(_get_struct_Q().pack(_x))
-      length = len(self.fused_ids)
+      _x = self.port
+      buff.write(_get_struct_I().pack(_x))
+      length = len(self.sensors)
       buff.write(_struct_I.pack(length))
-      pattern = '<%sQ'%length
-      buff.write(struct.Struct(pattern).pack(*self.fused_ids))
-      _x = self
-      buff.write(_get_struct_3d().pack(_x.position.x, _x.position.y, _x.position.z))
-      buff.write(_get_struct_9f().pack(*self.pos_covariance))
-      _x = self
-      buff.write(_get_struct_f9df().pack(_x.accuracy, _x.velocity.x, _x.velocity.y, _x.velocity.z, _x.acceleration.linear.x, _x.acceleration.linear.y, _x.acceleration.linear.z, _x.acceleration.angular.x, _x.acceleration.angular.y, _x.acceleration.angular.z, _x.size))
-      _x = self.classification
-      length = len(_x)
-      if python3 or type(_x) == unicode:
-        _x = _x.encode('utf-8')
+      for val1 in self.sensors:
+        _x = val1.sensor_id
         length = len(_x)
-      buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-      length = len(self.zones)
-      buff.write(_struct_I.pack(length))
-      for val1 in self.zones:
-        _x = val1
-        buff.write(_get_struct_IB().pack(_x.zone_id, _x.allowed))
-        _v1 = val1.first_detected
-        _x = _v1
-        buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
-        _v2 = val1.last_detected
+        if python3 or type(_x) == unicode:
+          _x = _x.encode('utf-8')
+          length = len(_x)
+        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+        _x = val1.model
+        length = len(_x)
+        if python3 or type(_x) == unicode:
+          _x = _x.encode('utf-8')
+          length = len(_x)
+        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+        _x = val1.type
+        buff.write(_get_struct_I().pack(_x))
+        _v1 = val1.pose
+        _v2 = _v1.position
         _x = _v2
-        buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
-      _x = self
-      buff.write(_get_struct_3I().pack(_x.bounding_cylinder.header.seq, _x.bounding_cylinder.header.stamp.secs, _x.bounding_cylinder.header.stamp.nsecs))
-      _x = self.bounding_cylinder.header.frame_id
-      length = len(_x)
-      if python3 or type(_x) == unicode:
-        _x = _x.encode('utf-8')
-        length = len(_x)
-      buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-      _x = self.bounding_cylinder.ns
-      length = len(_x)
-      if python3 or type(_x) == unicode:
-        _x = _x.encode('utf-8')
-        length = len(_x)
-      buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-      _x = self
-      buff.write(_get_struct_3i10d4f2iB().pack(_x.bounding_cylinder.id, _x.bounding_cylinder.type, _x.bounding_cylinder.action, _x.bounding_cylinder.pose.position.x, _x.bounding_cylinder.pose.position.y, _x.bounding_cylinder.pose.position.z, _x.bounding_cylinder.pose.orientation.x, _x.bounding_cylinder.pose.orientation.y, _x.bounding_cylinder.pose.orientation.z, _x.bounding_cylinder.pose.orientation.w, _x.bounding_cylinder.scale.x, _x.bounding_cylinder.scale.y, _x.bounding_cylinder.scale.z, _x.bounding_cylinder.color.r, _x.bounding_cylinder.color.g, _x.bounding_cylinder.color.b, _x.bounding_cylinder.color.a, _x.bounding_cylinder.lifetime.secs, _x.bounding_cylinder.lifetime.nsecs, _x.bounding_cylinder.frame_locked))
-      length = len(self.bounding_cylinder.points)
-      buff.write(_struct_I.pack(length))
-      for val1 in self.bounding_cylinder.points:
-        _x = val1
         buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-      length = len(self.bounding_cylinder.colors)
-      buff.write(_struct_I.pack(length))
-      for val1 in self.bounding_cylinder.colors:
+        _v3 = _v1.orientation
+        _x = _v3
+        buff.write(_get_struct_4d().pack(_x.x, _x.y, _x.z, _x.w))
         _x = val1
-        buff.write(_get_struct_4f().pack(_x.r, _x.g, _x.b, _x.a))
-      _x = self.bounding_cylinder.text
-      length = len(_x)
-      if python3 or type(_x) == unicode:
-        _x = _x.encode('utf-8')
+        buff.write(_get_struct_f3IfB().pack(_x.azimuth, _x.image_width, _x.image_height, _x.frame_rate, _x.power, _x.calibrated))
+        _v4 = val1.state
+        _x = _v4
+        buff.write(_get_struct_3I().pack(_x.id, _x.state, _x.status))
+        _x = _v4.description
         length = len(_x)
-      buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-      _x = self.bounding_cylinder.mesh_resource
-      length = len(_x)
-      if python3 or type(_x) == unicode:
-        _x = _x.encode('utf-8')
+        if python3 or type(_x) == unicode:
+          _x = _x.encode('utf-8')
+          length = len(_x)
+        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+        _x = _v4.lastChange
+        buff.write(_get_struct_I().pack(_x))
+        length = len(_v4.metrics)
+        buff.write(_struct_I.pack(length))
+        for val3 in _v4.metrics:
+          _x = val3.name
+          length = len(_x)
+          if python3 or type(_x) == unicode:
+            _x = _x.encode('utf-8')
+            length = len(_x)
+          buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+          _x = val3.value
+          length = len(_x)
+          if python3 or type(_x) == unicode:
+            _x = _x.encode('utf-8')
+            length = len(_x)
+          buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+        _v5 = val1.imu
+        _x = _v5.heading
+        buff.write(_get_struct_f().pack(_x))
+        _x = _v5.device_id
+        length = len(_x)
+        if python3 or type(_x) == unicode:
+          _x = _x.encode('utf-8')
+          length = len(_x)
+        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+        _v6 = _v5.imu
+        _v7 = _v6.header
+        _x = _v7.seq
+        buff.write(_get_struct_I().pack(_x))
+        _v8 = _v7.stamp
+        _x = _v8
+        buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
+        _x = _v7.frame_id
         length = len(_x)
-      buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-      _x = self.bounding_cylinder.mesh_use_embedded_materials
-      buff.write(_get_struct_B().pack(_x))
+        if python3 or type(_x) == unicode:
+          _x = _x.encode('utf-8')
+          length = len(_x)
+        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+        _v9 = _v6.orientation
+        _x = _v9
+        buff.write(_get_struct_4d().pack(_x.x, _x.y, _x.z, _x.w))
+        buff.write(_get_struct_9d().pack(*_v6.orientation_covariance))
+        _v10 = _v6.angular_velocity
+        _x = _v10
+        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
+        buff.write(_get_struct_9d().pack(*_v6.angular_velocity_covariance))
+        _v11 = _v6.linear_acceleration
+        _x = _v11
+        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
+        buff.write(_get_struct_9d().pack(*_v6.linear_acceleration_covariance))
+        _v12 = _v5.magnetic_field
+        _x = _v12
+        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
+        _x = _v5
+        buff.write(_get_struct_2fB().pack(_x.roll, _x.pitch, _x.deviceCalibrated))
     except struct.error as se: self._check_types(struct.error("%s: '%s' when writing '%s'" % (type(se), str(se), str(locals().get('_x', self)))))
     except TypeError as te: self._check_types(ValueError("%s: '%s' when writing '%s'" % (type(te), str(te), str(locals().get('_x', self)))))
 
   def deserialize(self, str):
     """
     unpack serialized message in str into this message instance
     :param str: byte array of serialized message, ``str``
     """
     if python3:
       codecs.lookup_error("rosmsg").msg_type = self._type
     try:
-      if self.header is None:
-        self.header = std_msgs.msg.Header()
-      if self.position is None:
-        self.position = geometry_msgs.msg.Point()
-      if self.velocity is None:
-        self.velocity = geometry_msgs.msg.Vector3()
-      if self.acceleration is None:
-        self.acceleration = geometry_msgs.msg.Accel()
-      if self.zones is None:
-        self.zones = None
-      if self.bounding_cylinder is None:
-        self.bounding_cylinder = visualization_msgs.msg.Marker()
+      if self.sensors is None:
+        self.sensors = None
       end = 0
-      _x = self
       start = end
-      end += 12
-      (_x.header.seq, _x.header.stamp.secs, _x.header.stamp.nsecs,) = _get_struct_3I().unpack(str[start:end])
+      end += 4
+      (self.system_id,) = _get_struct_I().unpack(str[start:end])
       start = end
       end += 4
       (length,) = _struct_I.unpack(str[start:end])
       start = end
       end += length
       if python3:
-        self.header.frame_id = str[start:end].decode('utf-8', 'rosmsg')
+        self.ip_address = str[start:end].decode('utf-8', 'rosmsg')
       else:
-        self.header.frame_id = str[start:end]
-      start = end
-      end += 8
-      (self.object_id,) = _get_struct_Q().unpack(str[start:end])
-      start = end
-      end += 4
-      (length,) = _struct_I.unpack(str[start:end])
-      pattern = '<%sQ'%length
-      start = end
-      s = struct.Struct(pattern)
-      end += s.size
-      self.fused_ids = s.unpack(str[start:end])
-      _x = self
-      start = end
-      end += 24
-      (_x.position.x, _x.position.y, _x.position.z,) = _get_struct_3d().unpack(str[start:end])
-      start = end
-      end += 36
-      self.pos_covariance = _get_struct_9f().unpack(str[start:end])
-      _x = self
-      start = end
-      end += 80
-      (_x.accuracy, _x.velocity.x, _x.velocity.y, _x.velocity.z, _x.acceleration.linear.x, _x.acceleration.linear.y, _x.acceleration.linear.z, _x.acceleration.angular.x, _x.acceleration.angular.y, _x.acceleration.angular.z, _x.size,) = _get_struct_f9df().unpack(str[start:end])
+        self.ip_address = str[start:end]
       start = end
       end += 4
-      (length,) = _struct_I.unpack(str[start:end])
-      start = end
-      end += length
-      if python3:
-        self.classification = str[start:end].decode('utf-8', 'rosmsg')
-      else:
-        self.classification = str[start:end]
+      (self.port,) = _get_struct_I().unpack(str[start:end])
       start = end
       end += 4
       (length,) = _struct_I.unpack(str[start:end])
-      self.zones = []
+      self.sensors = []
       for i in range(0, length):
-        val1 = digitaleye_msgs.msg.ZoneObjectStatus()
+        val1 = digitaleye_msgs.msg.Sensor()
+        start = end
+        end += 4
+        (length,) = _struct_I.unpack(str[start:end])
+        start = end
+        end += length
+        if python3:
+          val1.sensor_id = str[start:end].decode('utf-8', 'rosmsg')
+        else:
+          val1.sensor_id = str[start:end]
+        start = end
+        end += 4
+        (length,) = _struct_I.unpack(str[start:end])
+        start = end
+        end += length
+        if python3:
+          val1.model = str[start:end].decode('utf-8', 'rosmsg')
+        else:
+          val1.model = str[start:end]
+        start = end
+        end += 4
+        (val1.type,) = _get_struct_I().unpack(str[start:end])
+        _v13 = val1.pose
+        _v14 = _v13.position
+        _x = _v14
+        start = end
+        end += 24
+        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
+        _v15 = _v13.orientation
+        _x = _v15
+        start = end
+        end += 32
+        (_x.x, _x.y, _x.z, _x.w,) = _get_struct_4d().unpack(str[start:end])
         _x = val1
         start = end
-        end += 5
-        (_x.zone_id, _x.allowed,) = _get_struct_IB().unpack(str[start:end])
-        val1.allowed = bool(val1.allowed)
-        _v3 = val1.first_detected
-        _x = _v3
+        end += 21
+        (_x.azimuth, _x.image_width, _x.image_height, _x.frame_rate, _x.power, _x.calibrated,) = _get_struct_f3IfB().unpack(str[start:end])
+        val1.calibrated = bool(val1.calibrated)
+        _v16 = val1.state
+        _x = _v16
         start = end
-        end += 8
-        (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
-        _v4 = val1.last_detected
-        _x = _v4
+        end += 12
+        (_x.id, _x.state, _x.status,) = _get_struct_3I().unpack(str[start:end])
+        start = end
+        end += 4
+        (length,) = _struct_I.unpack(str[start:end])
+        start = end
+        end += length
+        if python3:
+          _v16.description = str[start:end].decode('utf-8', 'rosmsg')
+        else:
+          _v16.description = str[start:end]
+        start = end
+        end += 4
+        (_v16.lastChange,) = _get_struct_I().unpack(str[start:end])
+        start = end
+        end += 4
+        (length,) = _struct_I.unpack(str[start:end])
+        _v16.metrics = []
+        for i in range(0, length):
+          val3 = digitaleye_msgs.msg.Metric()
+          start = end
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          start = end
+          end += length
+          if python3:
+            val3.name = str[start:end].decode('utf-8', 'rosmsg')
+          else:
+            val3.name = str[start:end]
+          start = end
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          start = end
+          end += length
+          if python3:
+            val3.value = str[start:end].decode('utf-8', 'rosmsg')
+          else:
+            val3.value = str[start:end]
+          _v16.metrics.append(val3)
+        _v17 = val1.imu
+        start = end
+        end += 4
+        (_v17.heading,) = _get_struct_f().unpack(str[start:end])
+        start = end
+        end += 4
+        (length,) = _struct_I.unpack(str[start:end])
+        start = end
+        end += length
+        if python3:
+          _v17.device_id = str[start:end].decode('utf-8', 'rosmsg')
+        else:
+          _v17.device_id = str[start:end]
+        _v18 = _v17.imu
+        _v19 = _v18.header
+        start = end
+        end += 4
+        (_v19.seq,) = _get_struct_I().unpack(str[start:end])
+        _v20 = _v19.stamp
+        _x = _v20
         start = end
         end += 8
         (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
-        self.zones.append(val1)
-      _x = self
-      start = end
-      end += 12
-      (_x.bounding_cylinder.header.seq, _x.bounding_cylinder.header.stamp.secs, _x.bounding_cylinder.header.stamp.nsecs,) = _get_struct_3I().unpack(str[start:end])
-      start = end
-      end += 4
-      (length,) = _struct_I.unpack(str[start:end])
-      start = end
-      end += length
-      if python3:
-        self.bounding_cylinder.header.frame_id = str[start:end].decode('utf-8', 'rosmsg')
-      else:
-        self.bounding_cylinder.header.frame_id = str[start:end]
-      start = end
-      end += 4
-      (length,) = _struct_I.unpack(str[start:end])
-      start = end
-      end += length
-      if python3:
-        self.bounding_cylinder.ns = str[start:end].decode('utf-8', 'rosmsg')
-      else:
-        self.bounding_cylinder.ns = str[start:end]
-      _x = self
-      start = end
-      end += 117
-      (_x.bounding_cylinder.id, _x.bounding_cylinder.type, _x.bounding_cylinder.action, _x.bounding_cylinder.pose.position.x, _x.bounding_cylinder.pose.position.y, _x.bounding_cylinder.pose.position.z, _x.bounding_cylinder.pose.orientation.x, _x.bounding_cylinder.pose.orientation.y, _x.bounding_cylinder.pose.orientation.z, _x.bounding_cylinder.pose.orientation.w, _x.bounding_cylinder.scale.x, _x.bounding_cylinder.scale.y, _x.bounding_cylinder.scale.z, _x.bounding_cylinder.color.r, _x.bounding_cylinder.color.g, _x.bounding_cylinder.color.b, _x.bounding_cylinder.color.a, _x.bounding_cylinder.lifetime.secs, _x.bounding_cylinder.lifetime.nsecs, _x.bounding_cylinder.frame_locked,) = _get_struct_3i10d4f2iB().unpack(str[start:end])
-      self.bounding_cylinder.frame_locked = bool(self.bounding_cylinder.frame_locked)
-      start = end
-      end += 4
-      (length,) = _struct_I.unpack(str[start:end])
-      self.bounding_cylinder.points = []
-      for i in range(0, length):
-        val1 = geometry_msgs.msg.Point()
-        _x = val1
+        start = end
+        end += 4
+        (length,) = _struct_I.unpack(str[start:end])
+        start = end
+        end += length
+        if python3:
+          _v19.frame_id = str[start:end].decode('utf-8', 'rosmsg')
+        else:
+          _v19.frame_id = str[start:end]
+        _v21 = _v18.orientation
+        _x = _v21
+        start = end
+        end += 32
+        (_x.x, _x.y, _x.z, _x.w,) = _get_struct_4d().unpack(str[start:end])
+        start = end
+        end += 72
+        _v18.orientation_covariance = _get_struct_9d().unpack(str[start:end])
+        _v22 = _v18.angular_velocity
+        _x = _v22
         start = end
         end += 24
         (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        self.bounding_cylinder.points.append(val1)
-      start = end
-      end += 4
-      (length,) = _struct_I.unpack(str[start:end])
-      self.bounding_cylinder.colors = []
-      for i in range(0, length):
-        val1 = std_msgs.msg.ColorRGBA()
-        _x = val1
         start = end
-        end += 16
-        (_x.r, _x.g, _x.b, _x.a,) = _get_struct_4f().unpack(str[start:end])
-        self.bounding_cylinder.colors.append(val1)
-      start = end
-      end += 4
-      (length,) = _struct_I.unpack(str[start:end])
-      start = end
-      end += length
-      if python3:
-        self.bounding_cylinder.text = str[start:end].decode('utf-8', 'rosmsg')
-      else:
-        self.bounding_cylinder.text = str[start:end]
-      start = end
-      end += 4
-      (length,) = _struct_I.unpack(str[start:end])
-      start = end
-      end += length
-      if python3:
-        self.bounding_cylinder.mesh_resource = str[start:end].decode('utf-8', 'rosmsg')
-      else:
-        self.bounding_cylinder.mesh_resource = str[start:end]
-      start = end
-      end += 1
-      (self.bounding_cylinder.mesh_use_embedded_materials,) = _get_struct_B().unpack(str[start:end])
-      self.bounding_cylinder.mesh_use_embedded_materials = bool(self.bounding_cylinder.mesh_use_embedded_materials)
+        end += 72
+        _v18.angular_velocity_covariance = _get_struct_9d().unpack(str[start:end])
+        _v23 = _v18.linear_acceleration
+        _x = _v23
+        start = end
+        end += 24
+        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
+        start = end
+        end += 72
+        _v18.linear_acceleration_covariance = _get_struct_9d().unpack(str[start:end])
+        _v24 = _v17.magnetic_field
+        _x = _v24
+        start = end
+        end += 24
+        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
+        _x = _v17
+        start = end
+        end += 9
+        (_x.roll, _x.pitch, _x.deviceCalibrated,) = _get_struct_2fB().unpack(str[start:end])
+        _v17.deviceCalibrated = bool(_v17.deviceCalibrated)
+        self.sensors.append(val1)
       return self
     except struct.error as e:
       raise genpy.DeserializationError(e)  # most likely buffer underfill
 
 
   def serialize_numpy(self, buff, numpy):
     """
     serialize message with numpy array types into buffer
     :param buff: buffer, ``StringIO``
     :param numpy: numpy python module
     """
     try:
-      _x = self
-      buff.write(_get_struct_3I().pack(_x.header.seq, _x.header.stamp.secs, _x.header.stamp.nsecs))
-      _x = self.header.frame_id
+      _x = self.system_id
+      buff.write(_get_struct_I().pack(_x))
+      _x = self.ip_address
       length = len(_x)
       if python3 or type(_x) == unicode:
         _x = _x.encode('utf-8')
         length = len(_x)
       buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-      _x = self.object_id
-      buff.write(_get_struct_Q().pack(_x))
-      length = len(self.fused_ids)
+      _x = self.port
+      buff.write(_get_struct_I().pack(_x))
+      length = len(self.sensors)
       buff.write(_struct_I.pack(length))
-      pattern = '<%sQ'%length
-      buff.write(self.fused_ids.tostring())
-      _x = self
-      buff.write(_get_struct_3d().pack(_x.position.x, _x.position.y, _x.position.z))
-      buff.write(self.pos_covariance.tostring())
-      _x = self
-      buff.write(_get_struct_f9df().pack(_x.accuracy, _x.velocity.x, _x.velocity.y, _x.velocity.z, _x.acceleration.linear.x, _x.acceleration.linear.y, _x.acceleration.linear.z, _x.acceleration.angular.x, _x.acceleration.angular.y, _x.acceleration.angular.z, _x.size))
-      _x = self.classification
-      length = len(_x)
-      if python3 or type(_x) == unicode:
-        _x = _x.encode('utf-8')
+      for val1 in self.sensors:
+        _x = val1.sensor_id
         length = len(_x)
-      buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-      length = len(self.zones)
-      buff.write(_struct_I.pack(length))
-      for val1 in self.zones:
-        _x = val1
-        buff.write(_get_struct_IB().pack(_x.zone_id, _x.allowed))
-        _v5 = val1.first_detected
-        _x = _v5
-        buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
-        _v6 = val1.last_detected
-        _x = _v6
+        if python3 or type(_x) == unicode:
+          _x = _x.encode('utf-8')
+          length = len(_x)
+        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+        _x = val1.model
+        length = len(_x)
+        if python3 or type(_x) == unicode:
+          _x = _x.encode('utf-8')
+          length = len(_x)
+        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+        _x = val1.type
+        buff.write(_get_struct_I().pack(_x))
+        _v25 = val1.pose
+        _v26 = _v25.position
+        _x = _v26
+        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
+        _v27 = _v25.orientation
+        _x = _v27
+        buff.write(_get_struct_4d().pack(_x.x, _x.y, _x.z, _x.w))
+        _x = val1
+        buff.write(_get_struct_f3IfB().pack(_x.azimuth, _x.image_width, _x.image_height, _x.frame_rate, _x.power, _x.calibrated))
+        _v28 = val1.state
+        _x = _v28
+        buff.write(_get_struct_3I().pack(_x.id, _x.state, _x.status))
+        _x = _v28.description
+        length = len(_x)
+        if python3 or type(_x) == unicode:
+          _x = _x.encode('utf-8')
+          length = len(_x)
+        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+        _x = _v28.lastChange
+        buff.write(_get_struct_I().pack(_x))
+        length = len(_v28.metrics)
+        buff.write(_struct_I.pack(length))
+        for val3 in _v28.metrics:
+          _x = val3.name
+          length = len(_x)
+          if python3 or type(_x) == unicode:
+            _x = _x.encode('utf-8')
+            length = len(_x)
+          buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+          _x = val3.value
+          length = len(_x)
+          if python3 or type(_x) == unicode:
+            _x = _x.encode('utf-8')
+            length = len(_x)
+          buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+        _v29 = val1.imu
+        _x = _v29.heading
+        buff.write(_get_struct_f().pack(_x))
+        _x = _v29.device_id
+        length = len(_x)
+        if python3 or type(_x) == unicode:
+          _x = _x.encode('utf-8')
+          length = len(_x)
+        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+        _v30 = _v29.imu
+        _v31 = _v30.header
+        _x = _v31.seq
+        buff.write(_get_struct_I().pack(_x))
+        _v32 = _v31.stamp
+        _x = _v32
         buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
-      _x = self
-      buff.write(_get_struct_3I().pack(_x.bounding_cylinder.header.seq, _x.bounding_cylinder.header.stamp.secs, _x.bounding_cylinder.header.stamp.nsecs))
-      _x = self.bounding_cylinder.header.frame_id
-      length = len(_x)
-      if python3 or type(_x) == unicode:
-        _x = _x.encode('utf-8')
-        length = len(_x)
-      buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-      _x = self.bounding_cylinder.ns
-      length = len(_x)
-      if python3 or type(_x) == unicode:
-        _x = _x.encode('utf-8')
+        _x = _v31.frame_id
         length = len(_x)
-      buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-      _x = self
-      buff.write(_get_struct_3i10d4f2iB().pack(_x.bounding_cylinder.id, _x.bounding_cylinder.type, _x.bounding_cylinder.action, _x.bounding_cylinder.pose.position.x, _x.bounding_cylinder.pose.position.y, _x.bounding_cylinder.pose.position.z, _x.bounding_cylinder.pose.orientation.x, _x.bounding_cylinder.pose.orientation.y, _x.bounding_cylinder.pose.orientation.z, _x.bounding_cylinder.pose.orientation.w, _x.bounding_cylinder.scale.x, _x.bounding_cylinder.scale.y, _x.bounding_cylinder.scale.z, _x.bounding_cylinder.color.r, _x.bounding_cylinder.color.g, _x.bounding_cylinder.color.b, _x.bounding_cylinder.color.a, _x.bounding_cylinder.lifetime.secs, _x.bounding_cylinder.lifetime.nsecs, _x.bounding_cylinder.frame_locked))
-      length = len(self.bounding_cylinder.points)
-      buff.write(_struct_I.pack(length))
-      for val1 in self.bounding_cylinder.points:
-        _x = val1
+        if python3 or type(_x) == unicode:
+          _x = _x.encode('utf-8')
+          length = len(_x)
+        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+        _v33 = _v30.orientation
+        _x = _v33
+        buff.write(_get_struct_4d().pack(_x.x, _x.y, _x.z, _x.w))
+        buff.write(_v30.orientation_covariance.tostring())
+        _v34 = _v30.angular_velocity
+        _x = _v34
         buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-      length = len(self.bounding_cylinder.colors)
-      buff.write(_struct_I.pack(length))
-      for val1 in self.bounding_cylinder.colors:
-        _x = val1
-        buff.write(_get_struct_4f().pack(_x.r, _x.g, _x.b, _x.a))
-      _x = self.bounding_cylinder.text
-      length = len(_x)
-      if python3 or type(_x) == unicode:
-        _x = _x.encode('utf-8')
-        length = len(_x)
-      buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-      _x = self.bounding_cylinder.mesh_resource
-      length = len(_x)
-      if python3 or type(_x) == unicode:
-        _x = _x.encode('utf-8')
-        length = len(_x)
-      buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-      _x = self.bounding_cylinder.mesh_use_embedded_materials
-      buff.write(_get_struct_B().pack(_x))
+        buff.write(_v30.angular_velocity_covariance.tostring())
+        _v35 = _v30.linear_acceleration
+        _x = _v35
+        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
+        buff.write(_v30.linear_acceleration_covariance.tostring())
+        _v36 = _v29.magnetic_field
+        _x = _v36
+        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
+        _x = _v29
+        buff.write(_get_struct_2fB().pack(_x.roll, _x.pitch, _x.deviceCalibrated))
     except struct.error as se: self._check_types(struct.error("%s: '%s' when writing '%s'" % (type(se), str(se), str(locals().get('_x', self)))))
     except TypeError as te: self._check_types(ValueError("%s: '%s' when writing '%s'" % (type(te), str(te), str(locals().get('_x', self)))))
 
   def deserialize_numpy(self, str, numpy):
     """
     unpack serialized message in str into this message instance using numpy for array types
     :param str: byte array of serialized message, ``str``
     :param numpy: numpy python module
     """
     if python3:
       codecs.lookup_error("rosmsg").msg_type = self._type
     try:
-      if self.header is None:
-        self.header = std_msgs.msg.Header()
-      if self.position is None:
-        self.position = geometry_msgs.msg.Point()
-      if self.velocity is None:
-        self.velocity = geometry_msgs.msg.Vector3()
-      if self.acceleration is None:
-        self.acceleration = geometry_msgs.msg.Accel()
-      if self.zones is None:
-        self.zones = None
-      if self.bounding_cylinder is None:
-        self.bounding_cylinder = visualization_msgs.msg.Marker()
+      if self.sensors is None:
+        self.sensors = None
       end = 0
-      _x = self
       start = end
-      end += 12
-      (_x.header.seq, _x.header.stamp.secs, _x.header.stamp.nsecs,) = _get_struct_3I().unpack(str[start:end])
+      end += 4
+      (self.system_id,) = _get_struct_I().unpack(str[start:end])
       start = end
       end += 4
       (length,) = _struct_I.unpack(str[start:end])
       start = end
       end += length
       if python3:
-        self.header.frame_id = str[start:end].decode('utf-8', 'rosmsg')
+        self.ip_address = str[start:end].decode('utf-8', 'rosmsg')
       else:
-        self.header.frame_id = str[start:end]
-      start = end
-      end += 8
-      (self.object_id,) = _get_struct_Q().unpack(str[start:end])
-      start = end
-      end += 4
-      (length,) = _struct_I.unpack(str[start:end])
-      pattern = '<%sQ'%length
-      start = end
-      s = struct.Struct(pattern)
-      end += s.size
-      self.fused_ids = numpy.frombuffer(str[start:end], dtype=numpy.uint64, count=length)
-      _x = self
-      start = end
-      end += 24
-      (_x.position.x, _x.position.y, _x.position.z,) = _get_struct_3d().unpack(str[start:end])
-      start = end
-      end += 36
-      self.pos_covariance = numpy.frombuffer(str[start:end], dtype=numpy.float32, count=9)
-      _x = self
-      start = end
-      end += 80
-      (_x.accuracy, _x.velocity.x, _x.velocity.y, _x.velocity.z, _x.acceleration.linear.x, _x.acceleration.linear.y, _x.acceleration.linear.z, _x.acceleration.angular.x, _x.acceleration.angular.y, _x.acceleration.angular.z, _x.size,) = _get_struct_f9df().unpack(str[start:end])
+        self.ip_address = str[start:end]
       start = end
       end += 4
-      (length,) = _struct_I.unpack(str[start:end])
-      start = end
-      end += length
-      if python3:
-        self.classification = str[start:end].decode('utf-8', 'rosmsg')
-      else:
-        self.classification = str[start:end]
+      (self.port,) = _get_struct_I().unpack(str[start:end])
       start = end
       end += 4
       (length,) = _struct_I.unpack(str[start:end])
-      self.zones = []
+      self.sensors = []
       for i in range(0, length):
-        val1 = digitaleye_msgs.msg.ZoneObjectStatus()
+        val1 = digitaleye_msgs.msg.Sensor()
+        start = end
+        end += 4
+        (length,) = _struct_I.unpack(str[start:end])
+        start = end
+        end += length
+        if python3:
+          val1.sensor_id = str[start:end].decode('utf-8', 'rosmsg')
+        else:
+          val1.sensor_id = str[start:end]
+        start = end
+        end += 4
+        (length,) = _struct_I.unpack(str[start:end])
+        start = end
+        end += length
+        if python3:
+          val1.model = str[start:end].decode('utf-8', 'rosmsg')
+        else:
+          val1.model = str[start:end]
+        start = end
+        end += 4
+        (val1.type,) = _get_struct_I().unpack(str[start:end])
+        _v37 = val1.pose
+        _v38 = _v37.position
+        _x = _v38
+        start = end
+        end += 24
+        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
+        _v39 = _v37.orientation
+        _x = _v39
+        start = end
+        end += 32
+        (_x.x, _x.y, _x.z, _x.w,) = _get_struct_4d().unpack(str[start:end])
         _x = val1
         start = end
-        end += 5
-        (_x.zone_id, _x.allowed,) = _get_struct_IB().unpack(str[start:end])
-        val1.allowed = bool(val1.allowed)
-        _v7 = val1.first_detected
-        _x = _v7
+        end += 21
+        (_x.azimuth, _x.image_width, _x.image_height, _x.frame_rate, _x.power, _x.calibrated,) = _get_struct_f3IfB().unpack(str[start:end])
+        val1.calibrated = bool(val1.calibrated)
+        _v40 = val1.state
+        _x = _v40
         start = end
-        end += 8
-        (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
-        _v8 = val1.last_detected
-        _x = _v8
+        end += 12
+        (_x.id, _x.state, _x.status,) = _get_struct_3I().unpack(str[start:end])
+        start = end
+        end += 4
+        (length,) = _struct_I.unpack(str[start:end])
+        start = end
+        end += length
+        if python3:
+          _v40.description = str[start:end].decode('utf-8', 'rosmsg')
+        else:
+          _v40.description = str[start:end]
+        start = end
+        end += 4
+        (_v40.lastChange,) = _get_struct_I().unpack(str[start:end])
+        start = end
+        end += 4
+        (length,) = _struct_I.unpack(str[start:end])
+        _v40.metrics = []
+        for i in range(0, length):
+          val3 = digitaleye_msgs.msg.Metric()
+          start = end
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          start = end
+          end += length
+          if python3:
+            val3.name = str[start:end].decode('utf-8', 'rosmsg')
+          else:
+            val3.name = str[start:end]
+          start = end
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          start = end
+          end += length
+          if python3:
+            val3.value = str[start:end].decode('utf-8', 'rosmsg')
+          else:
+            val3.value = str[start:end]
+          _v40.metrics.append(val3)
+        _v41 = val1.imu
+        start = end
+        end += 4
+        (_v41.heading,) = _get_struct_f().unpack(str[start:end])
+        start = end
+        end += 4
+        (length,) = _struct_I.unpack(str[start:end])
+        start = end
+        end += length
+        if python3:
+          _v41.device_id = str[start:end].decode('utf-8', 'rosmsg')
+        else:
+          _v41.device_id = str[start:end]
+        _v42 = _v41.imu
+        _v43 = _v42.header
+        start = end
+        end += 4
+        (_v43.seq,) = _get_struct_I().unpack(str[start:end])
+        _v44 = _v43.stamp
+        _x = _v44
         start = end
         end += 8
         (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
-        self.zones.append(val1)
-      _x = self
-      start = end
-      end += 12
-      (_x.bounding_cylinder.header.seq, _x.bounding_cylinder.header.stamp.secs, _x.bounding_cylinder.header.stamp.nsecs,) = _get_struct_3I().unpack(str[start:end])
-      start = end
-      end += 4
-      (length,) = _struct_I.unpack(str[start:end])
-      start = end
-      end += length
-      if python3:
-        self.bounding_cylinder.header.frame_id = str[start:end].decode('utf-8', 'rosmsg')
-      else:
-        self.bounding_cylinder.header.frame_id = str[start:end]
-      start = end
-      end += 4
-      (length,) = _struct_I.unpack(str[start:end])
-      start = end
-      end += length
-      if python3:
-        self.bounding_cylinder.ns = str[start:end].decode('utf-8', 'rosmsg')
-      else:
-        self.bounding_cylinder.ns = str[start:end]
-      _x = self
-      start = end
-      end += 117
-      (_x.bounding_cylinder.id, _x.bounding_cylinder.type, _x.bounding_cylinder.action, _x.bounding_cylinder.pose.position.x, _x.bounding_cylinder.pose.position.y, _x.bounding_cylinder.pose.position.z, _x.bounding_cylinder.pose.orientation.x, _x.bounding_cylinder.pose.orientation.y, _x.bounding_cylinder.pose.orientation.z, _x.bounding_cylinder.pose.orientation.w, _x.bounding_cylinder.scale.x, _x.bounding_cylinder.scale.y, _x.bounding_cylinder.scale.z, _x.bounding_cylinder.color.r, _x.bounding_cylinder.color.g, _x.bounding_cylinder.color.b, _x.bounding_cylinder.color.a, _x.bounding_cylinder.lifetime.secs, _x.bounding_cylinder.lifetime.nsecs, _x.bounding_cylinder.frame_locked,) = _get_struct_3i10d4f2iB().unpack(str[start:end])
-      self.bounding_cylinder.frame_locked = bool(self.bounding_cylinder.frame_locked)
-      start = end
-      end += 4
-      (length,) = _struct_I.unpack(str[start:end])
-      self.bounding_cylinder.points = []
-      for i in range(0, length):
-        val1 = geometry_msgs.msg.Point()
-        _x = val1
+        start = end
+        end += 4
+        (length,) = _struct_I.unpack(str[start:end])
+        start = end
+        end += length
+        if python3:
+          _v43.frame_id = str[start:end].decode('utf-8', 'rosmsg')
+        else:
+          _v43.frame_id = str[start:end]
+        _v45 = _v42.orientation
+        _x = _v45
+        start = end
+        end += 32
+        (_x.x, _x.y, _x.z, _x.w,) = _get_struct_4d().unpack(str[start:end])
+        start = end
+        end += 72
+        _v42.orientation_covariance = numpy.frombuffer(str[start:end], dtype=numpy.float64, count=9)
+        _v46 = _v42.angular_velocity
+        _x = _v46
         start = end
         end += 24
         (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        self.bounding_cylinder.points.append(val1)
-      start = end
-      end += 4
-      (length,) = _struct_I.unpack(str[start:end])
-      self.bounding_cylinder.colors = []
-      for i in range(0, length):
-        val1 = std_msgs.msg.ColorRGBA()
-        _x = val1
         start = end
-        end += 16
-        (_x.r, _x.g, _x.b, _x.a,) = _get_struct_4f().unpack(str[start:end])
-        self.bounding_cylinder.colors.append(val1)
-      start = end
-      end += 4
-      (length,) = _struct_I.unpack(str[start:end])
-      start = end
-      end += length
-      if python3:
-        self.bounding_cylinder.text = str[start:end].decode('utf-8', 'rosmsg')
-      else:
-        self.bounding_cylinder.text = str[start:end]
-      start = end
-      end += 4
-      (length,) = _struct_I.unpack(str[start:end])
-      start = end
-      end += length
-      if python3:
-        self.bounding_cylinder.mesh_resource = str[start:end].decode('utf-8', 'rosmsg')
-      else:
-        self.bounding_cylinder.mesh_resource = str[start:end]
-      start = end
-      end += 1
-      (self.bounding_cylinder.mesh_use_embedded_materials,) = _get_struct_B().unpack(str[start:end])
-      self.bounding_cylinder.mesh_use_embedded_materials = bool(self.bounding_cylinder.mesh_use_embedded_materials)
+        end += 72
+        _v42.angular_velocity_covariance = numpy.frombuffer(str[start:end], dtype=numpy.float64, count=9)
+        _v47 = _v42.linear_acceleration
+        _x = _v47
+        start = end
+        end += 24
+        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
+        start = end
+        end += 72
+        _v42.linear_acceleration_covariance = numpy.frombuffer(str[start:end], dtype=numpy.float64, count=9)
+        _v48 = _v41.magnetic_field
+        _x = _v48
+        start = end
+        end += 24
+        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
+        _x = _v41
+        start = end
+        end += 9
+        (_x.roll, _x.pitch, _x.deviceCalibrated,) = _get_struct_2fB().unpack(str[start:end])
+        _v41.deviceCalibrated = bool(_v41.deviceCalibrated)
+        self.sensors.append(val1)
       return self
     except struct.error as e:
       raise genpy.DeserializationError(e)  # most likely buffer underfill
 
 _struct_I = genpy.struct_I
 def _get_struct_I():
     global _struct_I
     return _struct_I
 _struct_2I = None
 def _get_struct_2I():
     global _struct_2I
     if _struct_2I is None:
         _struct_2I = struct.Struct("<2I")
     return _struct_2I
+_struct_2fB = None
+def _get_struct_2fB():
+    global _struct_2fB
+    if _struct_2fB is None:
+        _struct_2fB = struct.Struct("<2fB")
+    return _struct_2fB
 _struct_3I = None
 def _get_struct_3I():
     global _struct_3I
     if _struct_3I is None:
         _struct_3I = struct.Struct("<3I")
     return _struct_3I
 _struct_3d = None
 def _get_struct_3d():
     global _struct_3d
     if _struct_3d is None:
         _struct_3d = struct.Struct("<3d")
     return _struct_3d
-_struct_3i10d4f2iB = None
-def _get_struct_3i10d4f2iB():
-    global _struct_3i10d4f2iB
-    if _struct_3i10d4f2iB is None:
-        _struct_3i10d4f2iB = struct.Struct("<3i10d4f2iB")
-    return _struct_3i10d4f2iB
-_struct_4f = None
-def _get_struct_4f():
-    global _struct_4f
-    if _struct_4f is None:
-        _struct_4f = struct.Struct("<4f")
-    return _struct_4f
-_struct_9f = None
-def _get_struct_9f():
-    global _struct_9f
-    if _struct_9f is None:
-        _struct_9f = struct.Struct("<9f")
-    return _struct_9f
-_struct_B = None
-def _get_struct_B():
-    global _struct_B
-    if _struct_B is None:
-        _struct_B = struct.Struct("<B")
-    return _struct_B
-_struct_IB = None
-def _get_struct_IB():
-    global _struct_IB
-    if _struct_IB is None:
-        _struct_IB = struct.Struct("<IB")
-    return _struct_IB
-_struct_Q = None
-def _get_struct_Q():
-    global _struct_Q
-    if _struct_Q is None:
-        _struct_Q = struct.Struct("<Q")
-    return _struct_Q
-_struct_f9df = None
-def _get_struct_f9df():
-    global _struct_f9df
-    if _struct_f9df is None:
-        _struct_f9df = struct.Struct("<f9df")
-    return _struct_f9df
+_struct_4d = None
+def _get_struct_4d():
+    global _struct_4d
+    if _struct_4d is None:
+        _struct_4d = struct.Struct("<4d")
+    return _struct_4d
+_struct_9d = None
+def _get_struct_9d():
+    global _struct_9d
+    if _struct_9d is None:
+        _struct_9d = struct.Struct("<9d")
+    return _struct_9d
+_struct_f = None
+def _get_struct_f():
+    global _struct_f
+    if _struct_f is None:
+        _struct_f = struct.Struct("<f")
+    return _struct_f
+_struct_f3IfB = None
+def _get_struct_f3IfB():
+    global _struct_f3IfB
+    if _struct_f3IfB is None:
+        _struct_f3IfB = struct.Struct("<f3IfB")
+    return _struct_f3IfB
```

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_ObjectList.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_SystemState.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,1052 +1,1136 @@
 # This Python file uses the following encoding: utf-8
-"""autogenerated by genpy from digitaleye_msgs/ObjectList.msg. Do not edit."""
+"""autogenerated by genpy from digitaleye_msgs/SystemState.msg. Do not edit."""
 import codecs
 import sys
 python3 = True if sys.hexversion > 0x03000000 else False
 import genpy
 import struct
 
 import digitaleye_msgs.msg
-import genpy
 import geometry_msgs.msg
+import sensor_msgs.msg
 import std_msgs.msg
-import visualization_msgs.msg
 
-class ObjectList(genpy.Message):
-  _md5sum = "f1860269ed96ba6ad58e8b3de0619ddc"
-  _type = "digitaleye_msgs/ObjectList"
-  _has_header = True  # flag to mark the presence of a Header object
-  _full_text = """# List of objects reported within the Monitered Space
-
-# information on the time at which objects
-# were reported (epoch time) and their reference frame
-std_msgs/Header header
+class SystemState(genpy.Message):
+  _md5sum = "f373ec9b3610db5e16911fbb76684b9c"
+  _type = "digitaleye_msgs/SystemState"
+  _has_header = False  # flag to mark the presence of a Header object
+  _full_text = """# State of a system and its constituent subsystem(s)
+
+# state of the system
+digitaleye_msgs/State system
 
-# list of reported object(s)
-digitaleye_msgs/Object[] objects
+# list of the state(s) of the system’s constituent component(s)
+digitaleye_msgs/ComponentState[] components
 
 ================================================================================
-MSG: std_msgs/Header
-# Standard metadata for higher-level stamped data types.
-# This is generally used to communicate timestamped data 
-# in a particular coordinate frame.
-# 
-# sequence ID: consecutively increasing ID 
-uint32 seq
-#Two-integer timestamp that is expressed as:
-# * stamp.sec: seconds (stamp_secs) since epoch (in Python the variable is called 'secs')
-# * stamp.nsec: nanoseconds since stamp_secs (in Python the variable is called 'nsecs')
-# time-handling sugar is provided by the client library
-time stamp
-#Frame this data is associated with
-string frame_id
+MSG: digitaleye_msgs/State
+# Details of a system’s status
+
+# unique identifier of the system
+# whose status is being reported
+uint32 id
+
+# system’s current state within the 
+# DigitalEye state machine
+uint32 state
+
+# system’s substatus within the current state,
+# unique to each system
+uint32 status
+
+# description of the system’s current state/status
+string description
+
+# timestamp indicating last change in state or status
+# (epoch time in sec)
+uint32 lastChange
+
+# list of performance metrics associated with the
+# current state
+digitaleye_msgs/Metric[] metrics
+
+================================================================================
+MSG: digitaleye_msgs/Metric
+# Performance indicator for a subsystem,
+# component or sensor
+
+# name of the performance indicator
+string name
+
+# value of the performance indicator
+string value
 
 ================================================================================
-MSG: digitaleye_msgs/Object
-# Description of an object in the Monitored Space
+MSG: digitaleye_msgs/ComponentState
+# State of a system component and its attached sensor(s)
 
-# information on the time at which the object
-# was reported (epoch time) and its reference frame
-std_msgs/Header header
+# state of the component
+digitaleye_msgs/State component
+
+# state(s) of the component’s attached sensor(s)
+digitaleye_msgs/Sensor[] sensors
+
+================================================================================
+MSG: digitaleye_msgs/Sensor
+# Description of a monitoring DigitalEye sensor
+# and its properties
 
-# id assigned to the reported object
-uint64 object_id
+# unique identifier of the sensor
+# e.g. hardware serial number
+string sensor_id
 
-# list of ID(s) of reported object(s) which
-# constitute it (if fused)
-uint64[] fused_ids
+# brand/model of sensor hardware
+string model
 
-# coordinates of the object’s estimated position
-# in the local reference frame (meters)
-geometry_msgs/Point position
+# type of sensor being described
+# e.g. camera, LIDAR, etc.
+uint32 type
 
-# 3D covariance of the object position, represents the quality
-# of the position estimate, higher covariances mean
-# a worse estimate. XX, XY, XZ, YX, YY, YZ, ZX, ZY, ZZ
-float32[9] pos_covariance
+# position of the sensor in
+# the DigitalEye’s local reference frame (meters)
+geometry_msgs/Pose pose
 
-# estimated accuracy radius of object's position (meters)
-float32 accuracy
+# direction in which the sensor is facing
+# with respect to the local frame’s x-axis
+float32 azimuth
 
-# estimated velocity of the object (m/s)
-geometry_msgs/Vector3 velocity
+# resolution height of the image captured by the sensor
+uint32 image_width
 
-# estimated acceleration of the object (m/s2)
-geometry_msgs/Accel acceleration
+# resolution width of the image captured by the sensor
+uint32 image_height
 
-# estimated size of the object (meters)
-float32 size
+# frame rate of a vision sensor
+uint32 frame_rate
 
-# object’s category
-# e.g. Personnel, Package, Passenger, UAV, etc.
-string classification
+# sensor’s current power level
+float32 power
 
-# list of zone(s) in which the object is
-ZoneObjectStatus[] zones
+# Whether or not the sensor has been calibrated
+bool calibrated
 
-# Object visualisation marker
-visualization_msgs/Marker bounding_cylinder
+# current state of the sensor
+digitaleye_msgs/State state
+
+# Sensor inertial measurements
+digitaleye_msgs/IMUValue imu
+
+================================================================================
+MSG: geometry_msgs/Pose
+# A representation of pose in free space, composed of position and orientation. 
+Point position
+Quaternion orientation
 
 ================================================================================
 MSG: geometry_msgs/Point
 # This contains the position of a point in free space
 float64 x
 float64 y
 float64 z
 
 ================================================================================
-MSG: geometry_msgs/Vector3
-# This represents a vector in free space. 
-# It is only meant to represent a direction. Therefore, it does not
-# make sense to apply a translation to it (e.g., when applying a 
-# generic rigid transformation to a Vector3, tf2 will only apply the
-# rotation). If you want your data to be translatable too, use the
-# geometry_msgs/Point message instead.
+MSG: geometry_msgs/Quaternion
+# This represents an orientation in free space in quaternion form.
 
 float64 x
 float64 y
 float64 z
-================================================================================
-MSG: geometry_msgs/Accel
-# This expresses acceleration in free space broken into its linear and angular parts.
-Vector3  linear
-Vector3  angular
+float64 w
 
 ================================================================================
-MSG: digitaleye_msgs/ZoneObjectStatus
-# Status of the object within the specified zone
+MSG: digitaleye_msgs/IMUValue
+# Description of an IMU value reading
 
-# identifier of the zone the object is in
-uint32 zone_id
+# Imu heading
+float32 heading
 
-# whether or not the object is allowed in the zone
-bool allowed
+# Unique identifier of the sensor
+# e.g. hardware serial number
+string device_id
 
-# time the object was first detected in this zone
-# (ros timestamp in epoch time)
-time first_detected
-
-# time the object was last detected in this zone
-# (ros timestamp in epoch time)
-time last_detected
+# Imu measurements
+sensor_msgs/Imu imu
+
+# Magenetometer readings
+geometry_msgs/Vector3 magnetic_field
+
+# Imu reading of roll
+float32 roll
+
+# Imu reading of pitch
+float32 pitch
+
+# Calibration status
+bool deviceCalibrated
 
 ================================================================================
-MSG: visualization_msgs/Marker
-# See http://www.ros.org/wiki/rviz/DisplayTypes/Marker and http://www.ros.org/wiki/rviz/Tutorials/Markers%3A%20Basic%20Shapes for more information on using this message with rviz
+MSG: sensor_msgs/Imu
+# This is a message to hold data from an IMU (Inertial Measurement Unit)
+#
+# Accelerations should be in m/s^2 (not in g's), and rotational velocity should be in rad/sec
+#
+# If the covariance of the measurement is known, it should be filled in (if all you know is the 
+# variance of each measurement, e.g. from the datasheet, just put those along the diagonal)
+# A covariance matrix of all zeros will be interpreted as "covariance unknown", and to use the
+# data a covariance will have to be assumed or gotten from some other source
+#
+# If you have no estimate for one of the data elements (e.g. your IMU doesn't produce an orientation 
+# estimate), please set element 0 of the associated covariance matrix to -1
+# If you are interpreting this message, please check for a value of -1 in the first element of each 
+# covariance matrix, and disregard the associated estimate.
+
+Header header
+
+geometry_msgs/Quaternion orientation
+float64[9] orientation_covariance # Row major about x, y, z axes
 
-uint8 ARROW=0
-uint8 CUBE=1
-uint8 SPHERE=2
-uint8 CYLINDER=3
-uint8 LINE_STRIP=4
-uint8 LINE_LIST=5
-uint8 CUBE_LIST=6
-uint8 SPHERE_LIST=7
-uint8 POINTS=8
-uint8 TEXT_VIEW_FACING=9
-uint8 MESH_RESOURCE=10
-uint8 TRIANGLE_LIST=11
-
-uint8 ADD=0
-uint8 MODIFY=0
-uint8 DELETE=2
-uint8 DELETEALL=3
-
-Header header                        # header for time/frame information
-string ns                            # Namespace to place this object in... used in conjunction with id to create a unique name for the object
-int32 id 		                         # object ID useful in conjunction with the namespace for manipulating and deleting the object later
-int32 type 		                       # Type of object
-int32 action 	                       # 0 add/modify an object, 1 (deprecated), 2 deletes an object, 3 deletes all objects
-geometry_msgs/Pose pose                 # Pose of the object
-geometry_msgs/Vector3 scale             # Scale of the object 1,1,1 means default (usually 1 meter square)
-std_msgs/ColorRGBA color             # Color [0.0-1.0]
-duration lifetime                    # How long the object should last before being automatically deleted.  0 means forever
-bool frame_locked                    # If this marker should be frame-locked, i.e. retransformed into its frame every timestep
-
-#Only used if the type specified has some use for them (eg. POINTS, LINE_STRIP, ...)
-geometry_msgs/Point[] points
-#Only used if the type specified has some use for them (eg. POINTS, LINE_STRIP, ...)
-#number of colors must either be 0 or equal to the number of points
-#NOTE: alpha is not yet used
-std_msgs/ColorRGBA[] colors
-
-# NOTE: only used for text markers
-string text
-
-# NOTE: only used for MESH_RESOURCE markers
-string mesh_resource
-bool mesh_use_embedded_materials
+geometry_msgs/Vector3 angular_velocity
+float64[9] angular_velocity_covariance # Row major about x, y, z axes
+
+geometry_msgs/Vector3 linear_acceleration
+float64[9] linear_acceleration_covariance # Row major x, y z 
 
 ================================================================================
-MSG: geometry_msgs/Pose
-# A representation of pose in free space, composed of position and orientation. 
-Point position
-Quaternion orientation
+MSG: std_msgs/Header
+# Standard metadata for higher-level stamped data types.
+# This is generally used to communicate timestamped data 
+# in a particular coordinate frame.
+# 
+# sequence ID: consecutively increasing ID 
+uint32 seq
+#Two-integer timestamp that is expressed as:
+# * stamp.sec: seconds (stamp_secs) since epoch (in Python the variable is called 'secs')
+# * stamp.nsec: nanoseconds since stamp_secs (in Python the variable is called 'nsecs')
+# time-handling sugar is provided by the client library
+time stamp
+#Frame this data is associated with
+string frame_id
 
 ================================================================================
-MSG: geometry_msgs/Quaternion
-# This represents an orientation in free space in quaternion form.
+MSG: geometry_msgs/Vector3
+# This represents a vector in free space. 
+# It is only meant to represent a direction. Therefore, it does not
+# make sense to apply a translation to it (e.g., when applying a 
+# generic rigid transformation to a Vector3, tf2 will only apply the
+# rotation). If you want your data to be translatable too, use the
+# geometry_msgs/Point message instead.
 
 float64 x
 float64 y
-float64 z
-float64 w
-
-================================================================================
-MSG: std_msgs/ColorRGBA
-float32 r
-float32 g
-float32 b
-float32 a
-"""
-  __slots__ = ['header','objects']
-  _slot_types = ['std_msgs/Header','digitaleye_msgs/Object[]']
+float64 z"""
+  __slots__ = ['system','components']
+  _slot_types = ['digitaleye_msgs/State','digitaleye_msgs/ComponentState[]']
 
   def __init__(self, *args, **kwds):
     """
     Constructor. Any message fields that are implicitly/explicitly
     set to None will be assigned a default value. The recommend
     use is keyword arguments as this is more robust to future message
     changes.  You cannot mix in-order arguments and keyword arguments.
 
     The available fields are:
-       header,objects
+       system,components
 
     :param args: complete set of field values, in .msg order
     :param kwds: use keyword arguments corresponding to message field names
     to set specific fields.
     """
     if args or kwds:
-      super(ObjectList, self).__init__(*args, **kwds)
+      super(SystemState, self).__init__(*args, **kwds)
       # message fields cannot be None, assign default values for those that are
-      if self.header is None:
-        self.header = std_msgs.msg.Header()
-      if self.objects is None:
-        self.objects = []
+      if self.system is None:
+        self.system = digitaleye_msgs.msg.State()
+      if self.components is None:
+        self.components = []
     else:
-      self.header = std_msgs.msg.Header()
-      self.objects = []
+      self.system = digitaleye_msgs.msg.State()
+      self.components = []
 
   def _get_types(self):
     """
     internal API method
     """
     return self._slot_types
 
   def serialize(self, buff):
     """
     serialize message into buffer
     :param buff: buffer, ``StringIO``
     """
     try:
       _x = self
-      buff.write(_get_struct_3I().pack(_x.header.seq, _x.header.stamp.secs, _x.header.stamp.nsecs))
-      _x = self.header.frame_id
+      buff.write(_get_struct_3I().pack(_x.system.id, _x.system.state, _x.system.status))
+      _x = self.system.description
       length = len(_x)
       if python3 or type(_x) == unicode:
         _x = _x.encode('utf-8')
         length = len(_x)
       buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-      length = len(self.objects)
+      _x = self.system.lastChange
+      buff.write(_get_struct_I().pack(_x))
+      length = len(self.system.metrics)
       buff.write(_struct_I.pack(length))
-      for val1 in self.objects:
-        _v1 = val1.header
-        _x = _v1.seq
-        buff.write(_get_struct_I().pack(_x))
-        _v2 = _v1.stamp
-        _x = _v2
-        buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
-        _x = _v1.frame_id
+      for val1 in self.system.metrics:
+        _x = val1.name
         length = len(_x)
         if python3 or type(_x) == unicode:
           _x = _x.encode('utf-8')
           length = len(_x)
         buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = val1.object_id
-        buff.write(_get_struct_Q().pack(_x))
-        length = len(val1.fused_ids)
-        buff.write(_struct_I.pack(length))
-        pattern = '<%sQ'%length
-        buff.write(struct.Struct(pattern).pack(*val1.fused_ids))
-        _v3 = val1.position
-        _x = _v3
-        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        buff.write(_get_struct_9f().pack(*val1.pos_covariance))
-        _x = val1.accuracy
-        buff.write(_get_struct_f().pack(_x))
-        _v4 = val1.velocity
-        _x = _v4
-        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        _v5 = val1.acceleration
-        _v6 = _v5.linear
-        _x = _v6
-        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        _v7 = _v5.angular
-        _x = _v7
-        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        _x = val1.size
-        buff.write(_get_struct_f().pack(_x))
-        _x = val1.classification
+        _x = val1.value
         length = len(_x)
         if python3 or type(_x) == unicode:
           _x = _x.encode('utf-8')
           length = len(_x)
         buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        length = len(val1.zones)
-        buff.write(_struct_I.pack(length))
-        for val2 in val1.zones:
-          _x = val2
-          buff.write(_get_struct_IB().pack(_x.zone_id, _x.allowed))
-          _v8 = val2.first_detected
-          _x = _v8
-          buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
-          _v9 = val2.last_detected
-          _x = _v9
-          buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
-        _v10 = val1.bounding_cylinder
-        _v11 = _v10.header
-        _x = _v11.seq
-        buff.write(_get_struct_I().pack(_x))
-        _v12 = _v11.stamp
-        _x = _v12
-        buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
-        _x = _v11.frame_id
+      length = len(self.components)
+      buff.write(_struct_I.pack(length))
+      for val1 in self.components:
+        _v1 = val1.component
+        _x = _v1
+        buff.write(_get_struct_3I().pack(_x.id, _x.state, _x.status))
+        _x = _v1.description
         length = len(_x)
         if python3 or type(_x) == unicode:
           _x = _x.encode('utf-8')
           length = len(_x)
         buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = _v10.ns
-        length = len(_x)
-        if python3 or type(_x) == unicode:
-          _x = _x.encode('utf-8')
+        _x = _v1.lastChange
+        buff.write(_get_struct_I().pack(_x))
+        length = len(_v1.metrics)
+        buff.write(_struct_I.pack(length))
+        for val3 in _v1.metrics:
+          _x = val3.name
           length = len(_x)
-        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = _v10
-        buff.write(_get_struct_3i().pack(_x.id, _x.type, _x.action))
-        _v13 = _v10.pose
-        _v14 = _v13.position
-        _x = _v14
-        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        _v15 = _v13.orientation
-        _x = _v15
-        buff.write(_get_struct_4d().pack(_x.x, _x.y, _x.z, _x.w))
-        _v16 = _v10.scale
-        _x = _v16
-        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        _v17 = _v10.color
-        _x = _v17
-        buff.write(_get_struct_4f().pack(_x.r, _x.g, _x.b, _x.a))
-        _v18 = _v10.lifetime
-        _x = _v18
-        buff.write(_get_struct_2i().pack(_x.secs, _x.nsecs))
-        _x = _v10.frame_locked
-        buff.write(_get_struct_B().pack(_x))
-        length = len(_v10.points)
+          if python3 or type(_x) == unicode:
+            _x = _x.encode('utf-8')
+            length = len(_x)
+          buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+          _x = val3.value
+          length = len(_x)
+          if python3 or type(_x) == unicode:
+            _x = _x.encode('utf-8')
+            length = len(_x)
+          buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+        length = len(val1.sensors)
         buff.write(_struct_I.pack(length))
-        for val3 in _v10.points:
-          _x = val3
+        for val2 in val1.sensors:
+          _x = val2.sensor_id
+          length = len(_x)
+          if python3 or type(_x) == unicode:
+            _x = _x.encode('utf-8')
+            length = len(_x)
+          buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+          _x = val2.model
+          length = len(_x)
+          if python3 or type(_x) == unicode:
+            _x = _x.encode('utf-8')
+            length = len(_x)
+          buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+          _x = val2.type
+          buff.write(_get_struct_I().pack(_x))
+          _v2 = val2.pose
+          _v3 = _v2.position
+          _x = _v3
           buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        length = len(_v10.colors)
-        buff.write(_struct_I.pack(length))
-        for val3 in _v10.colors:
-          _x = val3
-          buff.write(_get_struct_4f().pack(_x.r, _x.g, _x.b, _x.a))
-        _x = _v10.text
-        length = len(_x)
-        if python3 or type(_x) == unicode:
-          _x = _x.encode('utf-8')
+          _v4 = _v2.orientation
+          _x = _v4
+          buff.write(_get_struct_4d().pack(_x.x, _x.y, _x.z, _x.w))
+          _x = val2
+          buff.write(_get_struct_f3IfB().pack(_x.azimuth, _x.image_width, _x.image_height, _x.frame_rate, _x.power, _x.calibrated))
+          _v5 = val2.state
+          _x = _v5
+          buff.write(_get_struct_3I().pack(_x.id, _x.state, _x.status))
+          _x = _v5.description
           length = len(_x)
-        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = _v10.mesh_resource
-        length = len(_x)
-        if python3 or type(_x) == unicode:
-          _x = _x.encode('utf-8')
+          if python3 or type(_x) == unicode:
+            _x = _x.encode('utf-8')
+            length = len(_x)
+          buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+          _x = _v5.lastChange
+          buff.write(_get_struct_I().pack(_x))
+          length = len(_v5.metrics)
+          buff.write(_struct_I.pack(length))
+          for val4 in _v5.metrics:
+            _x = val4.name
+            length = len(_x)
+            if python3 or type(_x) == unicode:
+              _x = _x.encode('utf-8')
+              length = len(_x)
+            buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+            _x = val4.value
+            length = len(_x)
+            if python3 or type(_x) == unicode:
+              _x = _x.encode('utf-8')
+              length = len(_x)
+            buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+          _v6 = val2.imu
+          _x = _v6.heading
+          buff.write(_get_struct_f().pack(_x))
+          _x = _v6.device_id
           length = len(_x)
-        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = _v10.mesh_use_embedded_materials
-        buff.write(_get_struct_B().pack(_x))
+          if python3 or type(_x) == unicode:
+            _x = _x.encode('utf-8')
+            length = len(_x)
+          buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+          _v7 = _v6.imu
+          _v8 = _v7.header
+          _x = _v8.seq
+          buff.write(_get_struct_I().pack(_x))
+          _v9 = _v8.stamp
+          _x = _v9
+          buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
+          _x = _v8.frame_id
+          length = len(_x)
+          if python3 or type(_x) == unicode:
+            _x = _x.encode('utf-8')
+            length = len(_x)
+          buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+          _v10 = _v7.orientation
+          _x = _v10
+          buff.write(_get_struct_4d().pack(_x.x, _x.y, _x.z, _x.w))
+          buff.write(_get_struct_9d().pack(*_v7.orientation_covariance))
+          _v11 = _v7.angular_velocity
+          _x = _v11
+          buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
+          buff.write(_get_struct_9d().pack(*_v7.angular_velocity_covariance))
+          _v12 = _v7.linear_acceleration
+          _x = _v12
+          buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
+          buff.write(_get_struct_9d().pack(*_v7.linear_acceleration_covariance))
+          _v13 = _v6.magnetic_field
+          _x = _v13
+          buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
+          _x = _v6
+          buff.write(_get_struct_2fB().pack(_x.roll, _x.pitch, _x.deviceCalibrated))
     except struct.error as se: self._check_types(struct.error("%s: '%s' when writing '%s'" % (type(se), str(se), str(locals().get('_x', self)))))
     except TypeError as te: self._check_types(ValueError("%s: '%s' when writing '%s'" % (type(te), str(te), str(locals().get('_x', self)))))
 
   def deserialize(self, str):
     """
     unpack serialized message in str into this message instance
     :param str: byte array of serialized message, ``str``
     """
     if python3:
       codecs.lookup_error("rosmsg").msg_type = self._type
     try:
-      if self.header is None:
-        self.header = std_msgs.msg.Header()
-      if self.objects is None:
-        self.objects = None
+      if self.system is None:
+        self.system = digitaleye_msgs.msg.State()
+      if self.components is None:
+        self.components = None
       end = 0
       _x = self
       start = end
       end += 12
-      (_x.header.seq, _x.header.stamp.secs, _x.header.stamp.nsecs,) = _get_struct_3I().unpack(str[start:end])
+      (_x.system.id, _x.system.state, _x.system.status,) = _get_struct_3I().unpack(str[start:end])
       start = end
       end += 4
       (length,) = _struct_I.unpack(str[start:end])
       start = end
       end += length
       if python3:
-        self.header.frame_id = str[start:end].decode('utf-8', 'rosmsg')
+        self.system.description = str[start:end].decode('utf-8', 'rosmsg')
       else:
-        self.header.frame_id = str[start:end]
+        self.system.description = str[start:end]
+      start = end
+      end += 4
+      (self.system.lastChange,) = _get_struct_I().unpack(str[start:end])
       start = end
       end += 4
       (length,) = _struct_I.unpack(str[start:end])
-      self.objects = []
+      self.system.metrics = []
       for i in range(0, length):
-        val1 = digitaleye_msgs.msg.Object()
-        _v19 = val1.header
-        start = end
-        end += 4
-        (_v19.seq,) = _get_struct_I().unpack(str[start:end])
-        _v20 = _v19.stamp
-        _x = _v20
-        start = end
-        end += 8
-        (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
+        val1 = digitaleye_msgs.msg.Metric()
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
         start = end
         end += length
         if python3:
-          _v19.frame_id = str[start:end].decode('utf-8', 'rosmsg')
+          val1.name = str[start:end].decode('utf-8', 'rosmsg')
         else:
-          _v19.frame_id = str[start:end]
-        start = end
-        end += 8
-        (val1.object_id,) = _get_struct_Q().unpack(str[start:end])
-        start = end
-        end += 4
-        (length,) = _struct_I.unpack(str[start:end])
-        pattern = '<%sQ'%length
-        start = end
-        s = struct.Struct(pattern)
-        end += s.size
-        val1.fused_ids = s.unpack(str[start:end])
-        _v21 = val1.position
-        _x = _v21
-        start = end
-        end += 24
-        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        start = end
-        end += 36
-        val1.pos_covariance = _get_struct_9f().unpack(str[start:end])
-        start = end
-        end += 4
-        (val1.accuracy,) = _get_struct_f().unpack(str[start:end])
-        _v22 = val1.velocity
-        _x = _v22
-        start = end
-        end += 24
-        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        _v23 = val1.acceleration
-        _v24 = _v23.linear
-        _x = _v24
-        start = end
-        end += 24
-        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        _v25 = _v23.angular
-        _x = _v25
-        start = end
-        end += 24
-        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        start = end
-        end += 4
-        (val1.size,) = _get_struct_f().unpack(str[start:end])
+          val1.name = str[start:end]
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
         start = end
         end += length
         if python3:
-          val1.classification = str[start:end].decode('utf-8', 'rosmsg')
+          val1.value = str[start:end].decode('utf-8', 'rosmsg')
         else:
-          val1.classification = str[start:end]
-        start = end
-        end += 4
-        (length,) = _struct_I.unpack(str[start:end])
-        val1.zones = []
-        for i in range(0, length):
-          val2 = digitaleye_msgs.msg.ZoneObjectStatus()
-          _x = val2
-          start = end
-          end += 5
-          (_x.zone_id, _x.allowed,) = _get_struct_IB().unpack(str[start:end])
-          val2.allowed = bool(val2.allowed)
-          _v26 = val2.first_detected
-          _x = _v26
-          start = end
-          end += 8
-          (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
-          _v27 = val2.last_detected
-          _x = _v27
-          start = end
-          end += 8
-          (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
-          val1.zones.append(val2)
-        _v28 = val1.bounding_cylinder
-        _v29 = _v28.header
-        start = end
-        end += 4
-        (_v29.seq,) = _get_struct_I().unpack(str[start:end])
-        _v30 = _v29.stamp
-        _x = _v30
+          val1.value = str[start:end]
+        self.system.metrics.append(val1)
+      start = end
+      end += 4
+      (length,) = _struct_I.unpack(str[start:end])
+      self.components = []
+      for i in range(0, length):
+        val1 = digitaleye_msgs.msg.ComponentState()
+        _v14 = val1.component
+        _x = _v14
         start = end
-        end += 8
-        (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
+        end += 12
+        (_x.id, _x.state, _x.status,) = _get_struct_3I().unpack(str[start:end])
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
         start = end
         end += length
         if python3:
-          _v29.frame_id = str[start:end].decode('utf-8', 'rosmsg')
+          _v14.description = str[start:end].decode('utf-8', 'rosmsg')
         else:
-          _v29.frame_id = str[start:end]
+          _v14.description = str[start:end]
         start = end
         end += 4
-        (length,) = _struct_I.unpack(str[start:end])
-        start = end
-        end += length
-        if python3:
-          _v28.ns = str[start:end].decode('utf-8', 'rosmsg')
-        else:
-          _v28.ns = str[start:end]
-        _x = _v28
-        start = end
-        end += 12
-        (_x.id, _x.type, _x.action,) = _get_struct_3i().unpack(str[start:end])
-        _v31 = _v28.pose
-        _v32 = _v31.position
-        _x = _v32
-        start = end
-        end += 24
-        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        _v33 = _v31.orientation
-        _x = _v33
-        start = end
-        end += 32
-        (_x.x, _x.y, _x.z, _x.w,) = _get_struct_4d().unpack(str[start:end])
-        _v34 = _v28.scale
-        _x = _v34
-        start = end
-        end += 24
-        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        _v35 = _v28.color
-        _x = _v35
-        start = end
-        end += 16
-        (_x.r, _x.g, _x.b, _x.a,) = _get_struct_4f().unpack(str[start:end])
-        _v36 = _v28.lifetime
-        _x = _v36
-        start = end
-        end += 8
-        (_x.secs, _x.nsecs,) = _get_struct_2i().unpack(str[start:end])
-        start = end
-        end += 1
-        (_v28.frame_locked,) = _get_struct_B().unpack(str[start:end])
-        _v28.frame_locked = bool(_v28.frame_locked)
+        (_v14.lastChange,) = _get_struct_I().unpack(str[start:end])
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
-        _v28.points = []
+        _v14.metrics = []
         for i in range(0, length):
-          val3 = geometry_msgs.msg.Point()
-          _x = val3
+          val3 = digitaleye_msgs.msg.Metric()
           start = end
-          end += 24
-          (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-          _v28.points.append(val3)
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          start = end
+          end += length
+          if python3:
+            val3.name = str[start:end].decode('utf-8', 'rosmsg')
+          else:
+            val3.name = str[start:end]
+          start = end
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          start = end
+          end += length
+          if python3:
+            val3.value = str[start:end].decode('utf-8', 'rosmsg')
+          else:
+            val3.value = str[start:end]
+          _v14.metrics.append(val3)
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
-        _v28.colors = []
+        val1.sensors = []
         for i in range(0, length):
-          val3 = std_msgs.msg.ColorRGBA()
-          _x = val3
+          val2 = digitaleye_msgs.msg.Sensor()
           start = end
-          end += 16
-          (_x.r, _x.g, _x.b, _x.a,) = _get_struct_4f().unpack(str[start:end])
-          _v28.colors.append(val3)
-        start = end
-        end += 4
-        (length,) = _struct_I.unpack(str[start:end])
-        start = end
-        end += length
-        if python3:
-          _v28.text = str[start:end].decode('utf-8', 'rosmsg')
-        else:
-          _v28.text = str[start:end]
-        start = end
-        end += 4
-        (length,) = _struct_I.unpack(str[start:end])
-        start = end
-        end += length
-        if python3:
-          _v28.mesh_resource = str[start:end].decode('utf-8', 'rosmsg')
-        else:
-          _v28.mesh_resource = str[start:end]
-        start = end
-        end += 1
-        (_v28.mesh_use_embedded_materials,) = _get_struct_B().unpack(str[start:end])
-        _v28.mesh_use_embedded_materials = bool(_v28.mesh_use_embedded_materials)
-        self.objects.append(val1)
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          start = end
+          end += length
+          if python3:
+            val2.sensor_id = str[start:end].decode('utf-8', 'rosmsg')
+          else:
+            val2.sensor_id = str[start:end]
+          start = end
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          start = end
+          end += length
+          if python3:
+            val2.model = str[start:end].decode('utf-8', 'rosmsg')
+          else:
+            val2.model = str[start:end]
+          start = end
+          end += 4
+          (val2.type,) = _get_struct_I().unpack(str[start:end])
+          _v15 = val2.pose
+          _v16 = _v15.position
+          _x = _v16
+          start = end
+          end += 24
+          (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
+          _v17 = _v15.orientation
+          _x = _v17
+          start = end
+          end += 32
+          (_x.x, _x.y, _x.z, _x.w,) = _get_struct_4d().unpack(str[start:end])
+          _x = val2
+          start = end
+          end += 21
+          (_x.azimuth, _x.image_width, _x.image_height, _x.frame_rate, _x.power, _x.calibrated,) = _get_struct_f3IfB().unpack(str[start:end])
+          val2.calibrated = bool(val2.calibrated)
+          _v18 = val2.state
+          _x = _v18
+          start = end
+          end += 12
+          (_x.id, _x.state, _x.status,) = _get_struct_3I().unpack(str[start:end])
+          start = end
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          start = end
+          end += length
+          if python3:
+            _v18.description = str[start:end].decode('utf-8', 'rosmsg')
+          else:
+            _v18.description = str[start:end]
+          start = end
+          end += 4
+          (_v18.lastChange,) = _get_struct_I().unpack(str[start:end])
+          start = end
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          _v18.metrics = []
+          for i in range(0, length):
+            val4 = digitaleye_msgs.msg.Metric()
+            start = end
+            end += 4
+            (length,) = _struct_I.unpack(str[start:end])
+            start = end
+            end += length
+            if python3:
+              val4.name = str[start:end].decode('utf-8', 'rosmsg')
+            else:
+              val4.name = str[start:end]
+            start = end
+            end += 4
+            (length,) = _struct_I.unpack(str[start:end])
+            start = end
+            end += length
+            if python3:
+              val4.value = str[start:end].decode('utf-8', 'rosmsg')
+            else:
+              val4.value = str[start:end]
+            _v18.metrics.append(val4)
+          _v19 = val2.imu
+          start = end
+          end += 4
+          (_v19.heading,) = _get_struct_f().unpack(str[start:end])
+          start = end
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          start = end
+          end += length
+          if python3:
+            _v19.device_id = str[start:end].decode('utf-8', 'rosmsg')
+          else:
+            _v19.device_id = str[start:end]
+          _v20 = _v19.imu
+          _v21 = _v20.header
+          start = end
+          end += 4
+          (_v21.seq,) = _get_struct_I().unpack(str[start:end])
+          _v22 = _v21.stamp
+          _x = _v22
+          start = end
+          end += 8
+          (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
+          start = end
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          start = end
+          end += length
+          if python3:
+            _v21.frame_id = str[start:end].decode('utf-8', 'rosmsg')
+          else:
+            _v21.frame_id = str[start:end]
+          _v23 = _v20.orientation
+          _x = _v23
+          start = end
+          end += 32
+          (_x.x, _x.y, _x.z, _x.w,) = _get_struct_4d().unpack(str[start:end])
+          start = end
+          end += 72
+          _v20.orientation_covariance = _get_struct_9d().unpack(str[start:end])
+          _v24 = _v20.angular_velocity
+          _x = _v24
+          start = end
+          end += 24
+          (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
+          start = end
+          end += 72
+          _v20.angular_velocity_covariance = _get_struct_9d().unpack(str[start:end])
+          _v25 = _v20.linear_acceleration
+          _x = _v25
+          start = end
+          end += 24
+          (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
+          start = end
+          end += 72
+          _v20.linear_acceleration_covariance = _get_struct_9d().unpack(str[start:end])
+          _v26 = _v19.magnetic_field
+          _x = _v26
+          start = end
+          end += 24
+          (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
+          _x = _v19
+          start = end
+          end += 9
+          (_x.roll, _x.pitch, _x.deviceCalibrated,) = _get_struct_2fB().unpack(str[start:end])
+          _v19.deviceCalibrated = bool(_v19.deviceCalibrated)
+          val1.sensors.append(val2)
+        self.components.append(val1)
       return self
     except struct.error as e:
       raise genpy.DeserializationError(e)  # most likely buffer underfill
 
 
   def serialize_numpy(self, buff, numpy):
     """
     serialize message with numpy array types into buffer
     :param buff: buffer, ``StringIO``
     :param numpy: numpy python module
     """
     try:
       _x = self
-      buff.write(_get_struct_3I().pack(_x.header.seq, _x.header.stamp.secs, _x.header.stamp.nsecs))
-      _x = self.header.frame_id
+      buff.write(_get_struct_3I().pack(_x.system.id, _x.system.state, _x.system.status))
+      _x = self.system.description
       length = len(_x)
       if python3 or type(_x) == unicode:
         _x = _x.encode('utf-8')
         length = len(_x)
       buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-      length = len(self.objects)
+      _x = self.system.lastChange
+      buff.write(_get_struct_I().pack(_x))
+      length = len(self.system.metrics)
       buff.write(_struct_I.pack(length))
-      for val1 in self.objects:
-        _v37 = val1.header
-        _x = _v37.seq
-        buff.write(_get_struct_I().pack(_x))
-        _v38 = _v37.stamp
-        _x = _v38
-        buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
-        _x = _v37.frame_id
+      for val1 in self.system.metrics:
+        _x = val1.name
         length = len(_x)
         if python3 or type(_x) == unicode:
           _x = _x.encode('utf-8')
           length = len(_x)
         buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = val1.object_id
-        buff.write(_get_struct_Q().pack(_x))
-        length = len(val1.fused_ids)
-        buff.write(_struct_I.pack(length))
-        pattern = '<%sQ'%length
-        buff.write(val1.fused_ids.tostring())
-        _v39 = val1.position
-        _x = _v39
-        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        buff.write(val1.pos_covariance.tostring())
-        _x = val1.accuracy
-        buff.write(_get_struct_f().pack(_x))
-        _v40 = val1.velocity
-        _x = _v40
-        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        _v41 = val1.acceleration
-        _v42 = _v41.linear
-        _x = _v42
-        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        _v43 = _v41.angular
-        _x = _v43
-        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        _x = val1.size
-        buff.write(_get_struct_f().pack(_x))
-        _x = val1.classification
+        _x = val1.value
         length = len(_x)
         if python3 or type(_x) == unicode:
           _x = _x.encode('utf-8')
           length = len(_x)
         buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        length = len(val1.zones)
-        buff.write(_struct_I.pack(length))
-        for val2 in val1.zones:
-          _x = val2
-          buff.write(_get_struct_IB().pack(_x.zone_id, _x.allowed))
-          _v44 = val2.first_detected
-          _x = _v44
-          buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
-          _v45 = val2.last_detected
-          _x = _v45
-          buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
-        _v46 = val1.bounding_cylinder
-        _v47 = _v46.header
-        _x = _v47.seq
-        buff.write(_get_struct_I().pack(_x))
-        _v48 = _v47.stamp
-        _x = _v48
-        buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
-        _x = _v47.frame_id
+      length = len(self.components)
+      buff.write(_struct_I.pack(length))
+      for val1 in self.components:
+        _v27 = val1.component
+        _x = _v27
+        buff.write(_get_struct_3I().pack(_x.id, _x.state, _x.status))
+        _x = _v27.description
         length = len(_x)
         if python3 or type(_x) == unicode:
           _x = _x.encode('utf-8')
           length = len(_x)
         buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = _v46.ns
-        length = len(_x)
-        if python3 or type(_x) == unicode:
-          _x = _x.encode('utf-8')
+        _x = _v27.lastChange
+        buff.write(_get_struct_I().pack(_x))
+        length = len(_v27.metrics)
+        buff.write(_struct_I.pack(length))
+        for val3 in _v27.metrics:
+          _x = val3.name
           length = len(_x)
-        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = _v46
-        buff.write(_get_struct_3i().pack(_x.id, _x.type, _x.action))
-        _v49 = _v46.pose
-        _v50 = _v49.position
-        _x = _v50
-        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        _v51 = _v49.orientation
-        _x = _v51
-        buff.write(_get_struct_4d().pack(_x.x, _x.y, _x.z, _x.w))
-        _v52 = _v46.scale
-        _x = _v52
-        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        _v53 = _v46.color
-        _x = _v53
-        buff.write(_get_struct_4f().pack(_x.r, _x.g, _x.b, _x.a))
-        _v54 = _v46.lifetime
-        _x = _v54
-        buff.write(_get_struct_2i().pack(_x.secs, _x.nsecs))
-        _x = _v46.frame_locked
-        buff.write(_get_struct_B().pack(_x))
-        length = len(_v46.points)
+          if python3 or type(_x) == unicode:
+            _x = _x.encode('utf-8')
+            length = len(_x)
+          buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+          _x = val3.value
+          length = len(_x)
+          if python3 or type(_x) == unicode:
+            _x = _x.encode('utf-8')
+            length = len(_x)
+          buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+        length = len(val1.sensors)
         buff.write(_struct_I.pack(length))
-        for val3 in _v46.points:
-          _x = val3
+        for val2 in val1.sensors:
+          _x = val2.sensor_id
+          length = len(_x)
+          if python3 or type(_x) == unicode:
+            _x = _x.encode('utf-8')
+            length = len(_x)
+          buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+          _x = val2.model
+          length = len(_x)
+          if python3 or type(_x) == unicode:
+            _x = _x.encode('utf-8')
+            length = len(_x)
+          buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+          _x = val2.type
+          buff.write(_get_struct_I().pack(_x))
+          _v28 = val2.pose
+          _v29 = _v28.position
+          _x = _v29
           buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        length = len(_v46.colors)
-        buff.write(_struct_I.pack(length))
-        for val3 in _v46.colors:
-          _x = val3
-          buff.write(_get_struct_4f().pack(_x.r, _x.g, _x.b, _x.a))
-        _x = _v46.text
-        length = len(_x)
-        if python3 or type(_x) == unicode:
-          _x = _x.encode('utf-8')
+          _v30 = _v28.orientation
+          _x = _v30
+          buff.write(_get_struct_4d().pack(_x.x, _x.y, _x.z, _x.w))
+          _x = val2
+          buff.write(_get_struct_f3IfB().pack(_x.azimuth, _x.image_width, _x.image_height, _x.frame_rate, _x.power, _x.calibrated))
+          _v31 = val2.state
+          _x = _v31
+          buff.write(_get_struct_3I().pack(_x.id, _x.state, _x.status))
+          _x = _v31.description
           length = len(_x)
-        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = _v46.mesh_resource
-        length = len(_x)
-        if python3 or type(_x) == unicode:
-          _x = _x.encode('utf-8')
+          if python3 or type(_x) == unicode:
+            _x = _x.encode('utf-8')
+            length = len(_x)
+          buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+          _x = _v31.lastChange
+          buff.write(_get_struct_I().pack(_x))
+          length = len(_v31.metrics)
+          buff.write(_struct_I.pack(length))
+          for val4 in _v31.metrics:
+            _x = val4.name
+            length = len(_x)
+            if python3 or type(_x) == unicode:
+              _x = _x.encode('utf-8')
+              length = len(_x)
+            buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+            _x = val4.value
+            length = len(_x)
+            if python3 or type(_x) == unicode:
+              _x = _x.encode('utf-8')
+              length = len(_x)
+            buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+          _v32 = val2.imu
+          _x = _v32.heading
+          buff.write(_get_struct_f().pack(_x))
+          _x = _v32.device_id
           length = len(_x)
-        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = _v46.mesh_use_embedded_materials
-        buff.write(_get_struct_B().pack(_x))
+          if python3 or type(_x) == unicode:
+            _x = _x.encode('utf-8')
+            length = len(_x)
+          buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+          _v33 = _v32.imu
+          _v34 = _v33.header
+          _x = _v34.seq
+          buff.write(_get_struct_I().pack(_x))
+          _v35 = _v34.stamp
+          _x = _v35
+          buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
+          _x = _v34.frame_id
+          length = len(_x)
+          if python3 or type(_x) == unicode:
+            _x = _x.encode('utf-8')
+            length = len(_x)
+          buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+          _v36 = _v33.orientation
+          _x = _v36
+          buff.write(_get_struct_4d().pack(_x.x, _x.y, _x.z, _x.w))
+          buff.write(_v33.orientation_covariance.tostring())
+          _v37 = _v33.angular_velocity
+          _x = _v37
+          buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
+          buff.write(_v33.angular_velocity_covariance.tostring())
+          _v38 = _v33.linear_acceleration
+          _x = _v38
+          buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
+          buff.write(_v33.linear_acceleration_covariance.tostring())
+          _v39 = _v32.magnetic_field
+          _x = _v39
+          buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
+          _x = _v32
+          buff.write(_get_struct_2fB().pack(_x.roll, _x.pitch, _x.deviceCalibrated))
     except struct.error as se: self._check_types(struct.error("%s: '%s' when writing '%s'" % (type(se), str(se), str(locals().get('_x', self)))))
     except TypeError as te: self._check_types(ValueError("%s: '%s' when writing '%s'" % (type(te), str(te), str(locals().get('_x', self)))))
 
   def deserialize_numpy(self, str, numpy):
     """
     unpack serialized message in str into this message instance using numpy for array types
     :param str: byte array of serialized message, ``str``
     :param numpy: numpy python module
     """
     if python3:
       codecs.lookup_error("rosmsg").msg_type = self._type
     try:
-      if self.header is None:
-        self.header = std_msgs.msg.Header()
-      if self.objects is None:
-        self.objects = None
+      if self.system is None:
+        self.system = digitaleye_msgs.msg.State()
+      if self.components is None:
+        self.components = None
       end = 0
       _x = self
       start = end
       end += 12
-      (_x.header.seq, _x.header.stamp.secs, _x.header.stamp.nsecs,) = _get_struct_3I().unpack(str[start:end])
+      (_x.system.id, _x.system.state, _x.system.status,) = _get_struct_3I().unpack(str[start:end])
       start = end
       end += 4
       (length,) = _struct_I.unpack(str[start:end])
       start = end
       end += length
       if python3:
-        self.header.frame_id = str[start:end].decode('utf-8', 'rosmsg')
+        self.system.description = str[start:end].decode('utf-8', 'rosmsg')
       else:
-        self.header.frame_id = str[start:end]
+        self.system.description = str[start:end]
+      start = end
+      end += 4
+      (self.system.lastChange,) = _get_struct_I().unpack(str[start:end])
       start = end
       end += 4
       (length,) = _struct_I.unpack(str[start:end])
-      self.objects = []
+      self.system.metrics = []
       for i in range(0, length):
-        val1 = digitaleye_msgs.msg.Object()
-        _v55 = val1.header
-        start = end
-        end += 4
-        (_v55.seq,) = _get_struct_I().unpack(str[start:end])
-        _v56 = _v55.stamp
-        _x = _v56
-        start = end
-        end += 8
-        (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
+        val1 = digitaleye_msgs.msg.Metric()
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
         start = end
         end += length
         if python3:
-          _v55.frame_id = str[start:end].decode('utf-8', 'rosmsg')
+          val1.name = str[start:end].decode('utf-8', 'rosmsg')
         else:
-          _v55.frame_id = str[start:end]
-        start = end
-        end += 8
-        (val1.object_id,) = _get_struct_Q().unpack(str[start:end])
-        start = end
-        end += 4
-        (length,) = _struct_I.unpack(str[start:end])
-        pattern = '<%sQ'%length
-        start = end
-        s = struct.Struct(pattern)
-        end += s.size
-        val1.fused_ids = numpy.frombuffer(str[start:end], dtype=numpy.uint64, count=length)
-        _v57 = val1.position
-        _x = _v57
-        start = end
-        end += 24
-        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        start = end
-        end += 36
-        val1.pos_covariance = numpy.frombuffer(str[start:end], dtype=numpy.float32, count=9)
-        start = end
-        end += 4
-        (val1.accuracy,) = _get_struct_f().unpack(str[start:end])
-        _v58 = val1.velocity
-        _x = _v58
-        start = end
-        end += 24
-        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        _v59 = val1.acceleration
-        _v60 = _v59.linear
-        _x = _v60
-        start = end
-        end += 24
-        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        _v61 = _v59.angular
-        _x = _v61
-        start = end
-        end += 24
-        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        start = end
-        end += 4
-        (val1.size,) = _get_struct_f().unpack(str[start:end])
+          val1.name = str[start:end]
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
         start = end
         end += length
         if python3:
-          val1.classification = str[start:end].decode('utf-8', 'rosmsg')
+          val1.value = str[start:end].decode('utf-8', 'rosmsg')
         else:
-          val1.classification = str[start:end]
-        start = end
-        end += 4
-        (length,) = _struct_I.unpack(str[start:end])
-        val1.zones = []
-        for i in range(0, length):
-          val2 = digitaleye_msgs.msg.ZoneObjectStatus()
-          _x = val2
-          start = end
-          end += 5
-          (_x.zone_id, _x.allowed,) = _get_struct_IB().unpack(str[start:end])
-          val2.allowed = bool(val2.allowed)
-          _v62 = val2.first_detected
-          _x = _v62
-          start = end
-          end += 8
-          (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
-          _v63 = val2.last_detected
-          _x = _v63
-          start = end
-          end += 8
-          (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
-          val1.zones.append(val2)
-        _v64 = val1.bounding_cylinder
-        _v65 = _v64.header
-        start = end
-        end += 4
-        (_v65.seq,) = _get_struct_I().unpack(str[start:end])
-        _v66 = _v65.stamp
-        _x = _v66
+          val1.value = str[start:end]
+        self.system.metrics.append(val1)
+      start = end
+      end += 4
+      (length,) = _struct_I.unpack(str[start:end])
+      self.components = []
+      for i in range(0, length):
+        val1 = digitaleye_msgs.msg.ComponentState()
+        _v40 = val1.component
+        _x = _v40
         start = end
-        end += 8
-        (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
+        end += 12
+        (_x.id, _x.state, _x.status,) = _get_struct_3I().unpack(str[start:end])
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
         start = end
         end += length
         if python3:
-          _v65.frame_id = str[start:end].decode('utf-8', 'rosmsg')
+          _v40.description = str[start:end].decode('utf-8', 'rosmsg')
         else:
-          _v65.frame_id = str[start:end]
+          _v40.description = str[start:end]
         start = end
         end += 4
-        (length,) = _struct_I.unpack(str[start:end])
-        start = end
-        end += length
-        if python3:
-          _v64.ns = str[start:end].decode('utf-8', 'rosmsg')
-        else:
-          _v64.ns = str[start:end]
-        _x = _v64
-        start = end
-        end += 12
-        (_x.id, _x.type, _x.action,) = _get_struct_3i().unpack(str[start:end])
-        _v67 = _v64.pose
-        _v68 = _v67.position
-        _x = _v68
-        start = end
-        end += 24
-        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        _v69 = _v67.orientation
-        _x = _v69
-        start = end
-        end += 32
-        (_x.x, _x.y, _x.z, _x.w,) = _get_struct_4d().unpack(str[start:end])
-        _v70 = _v64.scale
-        _x = _v70
-        start = end
-        end += 24
-        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        _v71 = _v64.color
-        _x = _v71
-        start = end
-        end += 16
-        (_x.r, _x.g, _x.b, _x.a,) = _get_struct_4f().unpack(str[start:end])
-        _v72 = _v64.lifetime
-        _x = _v72
-        start = end
-        end += 8
-        (_x.secs, _x.nsecs,) = _get_struct_2i().unpack(str[start:end])
-        start = end
-        end += 1
-        (_v64.frame_locked,) = _get_struct_B().unpack(str[start:end])
-        _v64.frame_locked = bool(_v64.frame_locked)
+        (_v40.lastChange,) = _get_struct_I().unpack(str[start:end])
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
-        _v64.points = []
+        _v40.metrics = []
         for i in range(0, length):
-          val3 = geometry_msgs.msg.Point()
-          _x = val3
+          val3 = digitaleye_msgs.msg.Metric()
           start = end
-          end += 24
-          (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-          _v64.points.append(val3)
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          start = end
+          end += length
+          if python3:
+            val3.name = str[start:end].decode('utf-8', 'rosmsg')
+          else:
+            val3.name = str[start:end]
+          start = end
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          start = end
+          end += length
+          if python3:
+            val3.value = str[start:end].decode('utf-8', 'rosmsg')
+          else:
+            val3.value = str[start:end]
+          _v40.metrics.append(val3)
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
-        _v64.colors = []
+        val1.sensors = []
         for i in range(0, length):
-          val3 = std_msgs.msg.ColorRGBA()
-          _x = val3
+          val2 = digitaleye_msgs.msg.Sensor()
           start = end
-          end += 16
-          (_x.r, _x.g, _x.b, _x.a,) = _get_struct_4f().unpack(str[start:end])
-          _v64.colors.append(val3)
-        start = end
-        end += 4
-        (length,) = _struct_I.unpack(str[start:end])
-        start = end
-        end += length
-        if python3:
-          _v64.text = str[start:end].decode('utf-8', 'rosmsg')
-        else:
-          _v64.text = str[start:end]
-        start = end
-        end += 4
-        (length,) = _struct_I.unpack(str[start:end])
-        start = end
-        end += length
-        if python3:
-          _v64.mesh_resource = str[start:end].decode('utf-8', 'rosmsg')
-        else:
-          _v64.mesh_resource = str[start:end]
-        start = end
-        end += 1
-        (_v64.mesh_use_embedded_materials,) = _get_struct_B().unpack(str[start:end])
-        _v64.mesh_use_embedded_materials = bool(_v64.mesh_use_embedded_materials)
-        self.objects.append(val1)
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          start = end
+          end += length
+          if python3:
+            val2.sensor_id = str[start:end].decode('utf-8', 'rosmsg')
+          else:
+            val2.sensor_id = str[start:end]
+          start = end
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          start = end
+          end += length
+          if python3:
+            val2.model = str[start:end].decode('utf-8', 'rosmsg')
+          else:
+            val2.model = str[start:end]
+          start = end
+          end += 4
+          (val2.type,) = _get_struct_I().unpack(str[start:end])
+          _v41 = val2.pose
+          _v42 = _v41.position
+          _x = _v42
+          start = end
+          end += 24
+          (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
+          _v43 = _v41.orientation
+          _x = _v43
+          start = end
+          end += 32
+          (_x.x, _x.y, _x.z, _x.w,) = _get_struct_4d().unpack(str[start:end])
+          _x = val2
+          start = end
+          end += 21
+          (_x.azimuth, _x.image_width, _x.image_height, _x.frame_rate, _x.power, _x.calibrated,) = _get_struct_f3IfB().unpack(str[start:end])
+          val2.calibrated = bool(val2.calibrated)
+          _v44 = val2.state
+          _x = _v44
+          start = end
+          end += 12
+          (_x.id, _x.state, _x.status,) = _get_struct_3I().unpack(str[start:end])
+          start = end
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          start = end
+          end += length
+          if python3:
+            _v44.description = str[start:end].decode('utf-8', 'rosmsg')
+          else:
+            _v44.description = str[start:end]
+          start = end
+          end += 4
+          (_v44.lastChange,) = _get_struct_I().unpack(str[start:end])
+          start = end
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          _v44.metrics = []
+          for i in range(0, length):
+            val4 = digitaleye_msgs.msg.Metric()
+            start = end
+            end += 4
+            (length,) = _struct_I.unpack(str[start:end])
+            start = end
+            end += length
+            if python3:
+              val4.name = str[start:end].decode('utf-8', 'rosmsg')
+            else:
+              val4.name = str[start:end]
+            start = end
+            end += 4
+            (length,) = _struct_I.unpack(str[start:end])
+            start = end
+            end += length
+            if python3:
+              val4.value = str[start:end].decode('utf-8', 'rosmsg')
+            else:
+              val4.value = str[start:end]
+            _v44.metrics.append(val4)
+          _v45 = val2.imu
+          start = end
+          end += 4
+          (_v45.heading,) = _get_struct_f().unpack(str[start:end])
+          start = end
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          start = end
+          end += length
+          if python3:
+            _v45.device_id = str[start:end].decode('utf-8', 'rosmsg')
+          else:
+            _v45.device_id = str[start:end]
+          _v46 = _v45.imu
+          _v47 = _v46.header
+          start = end
+          end += 4
+          (_v47.seq,) = _get_struct_I().unpack(str[start:end])
+          _v48 = _v47.stamp
+          _x = _v48
+          start = end
+          end += 8
+          (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
+          start = end
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          start = end
+          end += length
+          if python3:
+            _v47.frame_id = str[start:end].decode('utf-8', 'rosmsg')
+          else:
+            _v47.frame_id = str[start:end]
+          _v49 = _v46.orientation
+          _x = _v49
+          start = end
+          end += 32
+          (_x.x, _x.y, _x.z, _x.w,) = _get_struct_4d().unpack(str[start:end])
+          start = end
+          end += 72
+          _v46.orientation_covariance = numpy.frombuffer(str[start:end], dtype=numpy.float64, count=9)
+          _v50 = _v46.angular_velocity
+          _x = _v50
+          start = end
+          end += 24
+          (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
+          start = end
+          end += 72
+          _v46.angular_velocity_covariance = numpy.frombuffer(str[start:end], dtype=numpy.float64, count=9)
+          _v51 = _v46.linear_acceleration
+          _x = _v51
+          start = end
+          end += 24
+          (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
+          start = end
+          end += 72
+          _v46.linear_acceleration_covariance = numpy.frombuffer(str[start:end], dtype=numpy.float64, count=9)
+          _v52 = _v45.magnetic_field
+          _x = _v52
+          start = end
+          end += 24
+          (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
+          _x = _v45
+          start = end
+          end += 9
+          (_x.roll, _x.pitch, _x.deviceCalibrated,) = _get_struct_2fB().unpack(str[start:end])
+          _v45.deviceCalibrated = bool(_v45.deviceCalibrated)
+          val1.sensors.append(val2)
+        self.components.append(val1)
       return self
     except struct.error as e:
       raise genpy.DeserializationError(e)  # most likely buffer underfill
 
 _struct_I = genpy.struct_I
 def _get_struct_I():
     global _struct_I
     return _struct_I
 _struct_2I = None
 def _get_struct_2I():
     global _struct_2I
     if _struct_2I is None:
         _struct_2I = struct.Struct("<2I")
     return _struct_2I
-_struct_2i = None
-def _get_struct_2i():
-    global _struct_2i
-    if _struct_2i is None:
-        _struct_2i = struct.Struct("<2i")
-    return _struct_2i
+_struct_2fB = None
+def _get_struct_2fB():
+    global _struct_2fB
+    if _struct_2fB is None:
+        _struct_2fB = struct.Struct("<2fB")
+    return _struct_2fB
 _struct_3I = None
 def _get_struct_3I():
     global _struct_3I
     if _struct_3I is None:
         _struct_3I = struct.Struct("<3I")
     return _struct_3I
 _struct_3d = None
 def _get_struct_3d():
     global _struct_3d
     if _struct_3d is None:
         _struct_3d = struct.Struct("<3d")
     return _struct_3d
-_struct_3i = None
-def _get_struct_3i():
-    global _struct_3i
-    if _struct_3i is None:
-        _struct_3i = struct.Struct("<3i")
-    return _struct_3i
 _struct_4d = None
 def _get_struct_4d():
     global _struct_4d
     if _struct_4d is None:
         _struct_4d = struct.Struct("<4d")
     return _struct_4d
-_struct_4f = None
-def _get_struct_4f():
-    global _struct_4f
-    if _struct_4f is None:
-        _struct_4f = struct.Struct("<4f")
-    return _struct_4f
-_struct_9f = None
-def _get_struct_9f():
-    global _struct_9f
-    if _struct_9f is None:
-        _struct_9f = struct.Struct("<9f")
-    return _struct_9f
-_struct_B = None
-def _get_struct_B():
-    global _struct_B
-    if _struct_B is None:
-        _struct_B = struct.Struct("<B")
-    return _struct_B
-_struct_IB = None
-def _get_struct_IB():
-    global _struct_IB
-    if _struct_IB is None:
-        _struct_IB = struct.Struct("<IB")
-    return _struct_IB
-_struct_Q = None
-def _get_struct_Q():
-    global _struct_Q
-    if _struct_Q is None:
-        _struct_Q = struct.Struct("<Q")
-    return _struct_Q
+_struct_9d = None
+def _get_struct_9d():
+    global _struct_9d
+    if _struct_9d is None:
+        _struct_9d = struct.Struct("<9d")
+    return _struct_9d
 _struct_f = None
 def _get_struct_f():
     global _struct_f
     if _struct_f is None:
         _struct_f = struct.Struct("<f")
     return _struct_f
+_struct_f3IfB = None
+def _get_struct_f3IfB():
+    global _struct_f3IfB
+    if _struct_f3IfB is None:
+        _struct_f3IfB = struct.Struct("<f3IfB")
+    return _struct_f3IfB
```

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Pause.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Pause.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Pole.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Pole.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_PolePose.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_PolePose.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Position.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Position.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Sector.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Sector.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_SectorPicture.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_SectorPicture.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Sensor.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Sensor.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_SensorPose.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_SensorPose.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_State.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_State.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_SystemCommand.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_SystemCommand.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_SystemConfiguration.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetStatus.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,192 @@
 # This Python file uses the following encoding: utf-8
-"""autogenerated by genpy from digitaleye_msgs/SystemConfiguration.msg. Do not edit."""
+"""autogenerated by genpy from digitaleye_msgs/GetStatusRequest.msg. Do not edit."""
+import codecs
+import sys
+python3 = True if sys.hexversion > 0x03000000 else False
+import genpy
+import struct
+
+
+class GetStatusRequest(genpy.Message):
+  _md5sum = "d41d8cd98f00b204e9800998ecf8427e"
+  _type = "digitaleye_msgs/GetStatusRequest"
+  _has_header = False  # flag to mark the presence of a Header object
+  _full_text = """"""
+  __slots__ = []
+  _slot_types = []
+
+  def __init__(self, *args, **kwds):
+    """
+    Constructor. Any message fields that are implicitly/explicitly
+    set to None will be assigned a default value. The recommend
+    use is keyword arguments as this is more robust to future message
+    changes.  You cannot mix in-order arguments and keyword arguments.
+
+    The available fields are:
+       
+
+    :param args: complete set of field values, in .msg order
+    :param kwds: use keyword arguments corresponding to message field names
+    to set specific fields.
+    """
+    if args or kwds:
+      super(GetStatusRequest, self).__init__(*args, **kwds)
+
+  def _get_types(self):
+    """
+    internal API method
+    """
+    return self._slot_types
+
+  def serialize(self, buff):
+    """
+    serialize message into buffer
+    :param buff: buffer, ``StringIO``
+    """
+    try:
+      pass
+    except struct.error as se: self._check_types(struct.error("%s: '%s' when writing '%s'" % (type(se), str(se), str(locals().get('_x', self)))))
+    except TypeError as te: self._check_types(ValueError("%s: '%s' when writing '%s'" % (type(te), str(te), str(locals().get('_x', self)))))
+
+  def deserialize(self, str):
+    """
+    unpack serialized message in str into this message instance
+    :param str: byte array of serialized message, ``str``
+    """
+    if python3:
+      codecs.lookup_error("rosmsg").msg_type = self._type
+    try:
+      end = 0
+      return self
+    except struct.error as e:
+      raise genpy.DeserializationError(e)  # most likely buffer underfill
+
+
+  def serialize_numpy(self, buff, numpy):
+    """
+    serialize message with numpy array types into buffer
+    :param buff: buffer, ``StringIO``
+    :param numpy: numpy python module
+    """
+    try:
+      pass
+    except struct.error as se: self._check_types(struct.error("%s: '%s' when writing '%s'" % (type(se), str(se), str(locals().get('_x', self)))))
+    except TypeError as te: self._check_types(ValueError("%s: '%s' when writing '%s'" % (type(te), str(te), str(locals().get('_x', self)))))
+
+  def deserialize_numpy(self, str, numpy):
+    """
+    unpack serialized message in str into this message instance using numpy for array types
+    :param str: byte array of serialized message, ``str``
+    :param numpy: numpy python module
+    """
+    if python3:
+      codecs.lookup_error("rosmsg").msg_type = self._type
+    try:
+      end = 0
+      return self
+    except struct.error as e:
+      raise genpy.DeserializationError(e)  # most likely buffer underfill
+
+_struct_I = genpy.struct_I
+def _get_struct_I():
+    global _struct_I
+    return _struct_I
+# This Python file uses the following encoding: utf-8
+"""autogenerated by genpy from digitaleye_msgs/GetStatusResponse.msg. Do not edit."""
 import codecs
 import sys
 python3 = True if sys.hexversion > 0x03000000 else False
 import genpy
 import struct
 
 import digitaleye_msgs.msg
 import geometry_msgs.msg
 import sensor_msgs.msg
 import std_msgs.msg
 
-class SystemConfiguration(genpy.Message):
-  _md5sum = "aa0494b2170d4b3eac19f93e9fcd5c9c"
-  _type = "digitaleye_msgs/SystemConfiguration"
+class GetStatusResponse(genpy.Message):
+  _md5sum = "3debe849e7d84e1c8a45738e73fc747e"
+  _type = "digitaleye_msgs/GetStatusResponse"
   _has_header = False  # flag to mark the presence of a Header object
-  _full_text = """# Configuration of a DigitalEye subsystem
+  _full_text = """# DigitalEye Operating Status
+digitaleye_msgs/DigitalEyeStatus status
+
+
+================================================================================
+MSG: digitaleye_msgs/DigitalEyeStatus
+# Details of the DigitalEye’s external state,
+# and the states of its subsystems
+
+# TODO
+uint32 started
+
+# current external state of the DigitalEye
+digitaleye_msgs/State digitaleye
+
+# states of the DigitalEye’s subsystem(s)
+# (DEMS, MVS , IOT, etc.) and their component(s)
+digitaleye_msgs/SystemState[] subsystems
+
+================================================================================
+MSG: digitaleye_msgs/State
+# Details of a system’s status
+
+# unique identifier of the system
+# whose status is being reported
+uint32 id
+
+# system’s current state within the 
+# DigitalEye state machine
+uint32 state
 
-# unique identifier of the configured subsystem
-uint32 system_id
+# system’s substatus within the current state,
+# unique to each system
+uint32 status
 
-# subsystem’s network IP address
-string ip_address
+# description of the system’s current state/status
+string description
 
-# port on which the subsystem is accepting
-# incoming connections from the DEMS
-uint32 port
+# timestamp indicating last change in state or status
+# (epoch time in sec)
+uint32 lastChange
+
+# list of performance metrics associated with the
+# current state
+digitaleye_msgs/Metric[] metrics
 
-# list of monitoring sensor(s) attached to this subsystem
+================================================================================
+MSG: digitaleye_msgs/Metric
+# Performance indicator for a subsystem,
+# component or sensor
+
+# name of the performance indicator
+string name
+
+# value of the performance indicator
+string value
+
+================================================================================
+MSG: digitaleye_msgs/SystemState
+# State of a system and its constituent subsystem(s)
+
+# state of the system
+digitaleye_msgs/State system
+
+# list of the state(s) of the system’s constituent component(s)
+digitaleye_msgs/ComponentState[] components
+
+================================================================================
+MSG: digitaleye_msgs/ComponentState
+# State of a system component and its attached sensor(s)
+
+# state of the component
+digitaleye_msgs/State component
+
+# state(s) of the component’s attached sensor(s)
 digitaleye_msgs/Sensor[] sensors
 
 ================================================================================
 MSG: digitaleye_msgs/Sensor
 # Description of a monitoring DigitalEye sensor
 # and its properties
 
@@ -94,52 +249,14 @@
 
 float64 x
 float64 y
 float64 z
 float64 w
 
 ================================================================================
-MSG: digitaleye_msgs/State
-# Details of a system’s status
-
-# unique identifier of the system
-# whose status is being reported
-uint32 id
-
-# system’s current state within the 
-# DigitalEye state machine
-uint32 state
-
-# system’s substatus within the current state,
-# unique to each system
-uint32 status
-
-# description of the system’s current state/status
-string description
-
-# timestamp indicating last change in state or status
-# (epoch time in sec)
-uint32 lastChange
-
-# list of performance metrics associated with the
-# current state
-digitaleye_msgs/Metric[] metrics
-
-================================================================================
-MSG: digitaleye_msgs/Metric
-# Performance indicator for a subsystem,
-# component or sensor
-
-# name of the performance indicator
-string name
-
-# value of the performance indicator
-string value
-
-================================================================================
 MSG: digitaleye_msgs/IMUValue
 # Description of an IMU value reading
 
 # Imu heading
 float32 heading
 
 # Unique identifier of the sensor
@@ -212,254 +329,307 @@
 # generic rigid transformation to a Vector3, tf2 will only apply the
 # rotation). If you want your data to be translatable too, use the
 # geometry_msgs/Point message instead.
 
 float64 x
 float64 y
 float64 z"""
-  __slots__ = ['system_id','ip_address','port','sensors']
-  _slot_types = ['uint32','string','uint32','digitaleye_msgs/Sensor[]']
+  __slots__ = ['status']
+  _slot_types = ['digitaleye_msgs/DigitalEyeStatus']
 
   def __init__(self, *args, **kwds):
     """
     Constructor. Any message fields that are implicitly/explicitly
     set to None will be assigned a default value. The recommend
     use is keyword arguments as this is more robust to future message
     changes.  You cannot mix in-order arguments and keyword arguments.
 
     The available fields are:
-       system_id,ip_address,port,sensors
+       status
 
     :param args: complete set of field values, in .msg order
     :param kwds: use keyword arguments corresponding to message field names
     to set specific fields.
     """
     if args or kwds:
-      super(SystemConfiguration, self).__init__(*args, **kwds)
+      super(GetStatusResponse, self).__init__(*args, **kwds)
       # message fields cannot be None, assign default values for those that are
-      if self.system_id is None:
-        self.system_id = 0
-      if self.ip_address is None:
-        self.ip_address = ''
-      if self.port is None:
-        self.port = 0
-      if self.sensors is None:
-        self.sensors = []
+      if self.status is None:
+        self.status = digitaleye_msgs.msg.DigitalEyeStatus()
     else:
-      self.system_id = 0
-      self.ip_address = ''
-      self.port = 0
-      self.sensors = []
+      self.status = digitaleye_msgs.msg.DigitalEyeStatus()
 
   def _get_types(self):
     """
     internal API method
     """
     return self._slot_types
 
   def serialize(self, buff):
     """
     serialize message into buffer
     :param buff: buffer, ``StringIO``
     """
     try:
-      _x = self.system_id
-      buff.write(_get_struct_I().pack(_x))
-      _x = self.ip_address
+      _x = self
+      buff.write(_get_struct_4I().pack(_x.status.started, _x.status.digitaleye.id, _x.status.digitaleye.state, _x.status.digitaleye.status))
+      _x = self.status.digitaleye.description
       length = len(_x)
       if python3 or type(_x) == unicode:
         _x = _x.encode('utf-8')
         length = len(_x)
       buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-      _x = self.port
+      _x = self.status.digitaleye.lastChange
       buff.write(_get_struct_I().pack(_x))
-      length = len(self.sensors)
+      length = len(self.status.digitaleye.metrics)
       buff.write(_struct_I.pack(length))
-      for val1 in self.sensors:
-        _x = val1.sensor_id
+      for val1 in self.status.digitaleye.metrics:
+        _x = val1.name
         length = len(_x)
         if python3 or type(_x) == unicode:
           _x = _x.encode('utf-8')
           length = len(_x)
         buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = val1.model
+        _x = val1.value
         length = len(_x)
         if python3 or type(_x) == unicode:
           _x = _x.encode('utf-8')
           length = len(_x)
         buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = val1.type
-        buff.write(_get_struct_I().pack(_x))
-        _v1 = val1.pose
-        _v2 = _v1.position
-        _x = _v2
-        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        _v3 = _v1.orientation
-        _x = _v3
-        buff.write(_get_struct_4d().pack(_x.x, _x.y, _x.z, _x.w))
-        _x = val1
-        buff.write(_get_struct_f3IfB().pack(_x.azimuth, _x.image_width, _x.image_height, _x.frame_rate, _x.power, _x.calibrated))
-        _v4 = val1.state
-        _x = _v4
+      length = len(self.status.subsystems)
+      buff.write(_struct_I.pack(length))
+      for val1 in self.status.subsystems:
+        _v1 = val1.system
+        _x = _v1
         buff.write(_get_struct_3I().pack(_x.id, _x.state, _x.status))
-        _x = _v4.description
+        _x = _v1.description
         length = len(_x)
         if python3 or type(_x) == unicode:
           _x = _x.encode('utf-8')
           length = len(_x)
         buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = _v4.lastChange
+        _x = _v1.lastChange
         buff.write(_get_struct_I().pack(_x))
-        length = len(_v4.metrics)
+        length = len(_v1.metrics)
         buff.write(_struct_I.pack(length))
-        for val3 in _v4.metrics:
+        for val3 in _v1.metrics:
           _x = val3.name
           length = len(_x)
           if python3 or type(_x) == unicode:
             _x = _x.encode('utf-8')
             length = len(_x)
           buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
           _x = val3.value
           length = len(_x)
           if python3 or type(_x) == unicode:
             _x = _x.encode('utf-8')
             length = len(_x)
           buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _v5 = val1.imu
-        _x = _v5.heading
-        buff.write(_get_struct_f().pack(_x))
-        _x = _v5.device_id
-        length = len(_x)
-        if python3 or type(_x) == unicode:
-          _x = _x.encode('utf-8')
-          length = len(_x)
-        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _v6 = _v5.imu
-        _v7 = _v6.header
-        _x = _v7.seq
-        buff.write(_get_struct_I().pack(_x))
-        _v8 = _v7.stamp
-        _x = _v8
-        buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
-        _x = _v7.frame_id
-        length = len(_x)
-        if python3 or type(_x) == unicode:
-          _x = _x.encode('utf-8')
+        length = len(val1.components)
+        buff.write(_struct_I.pack(length))
+        for val2 in val1.components:
+          _v2 = val2.component
+          _x = _v2
+          buff.write(_get_struct_3I().pack(_x.id, _x.state, _x.status))
+          _x = _v2.description
           length = len(_x)
-        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _v9 = _v6.orientation
-        _x = _v9
-        buff.write(_get_struct_4d().pack(_x.x, _x.y, _x.z, _x.w))
-        buff.write(_get_struct_9d().pack(*_v6.orientation_covariance))
-        _v10 = _v6.angular_velocity
-        _x = _v10
-        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        buff.write(_get_struct_9d().pack(*_v6.angular_velocity_covariance))
-        _v11 = _v6.linear_acceleration
-        _x = _v11
-        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        buff.write(_get_struct_9d().pack(*_v6.linear_acceleration_covariance))
-        _v12 = _v5.magnetic_field
-        _x = _v12
-        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        _x = _v5
-        buff.write(_get_struct_2fB().pack(_x.roll, _x.pitch, _x.deviceCalibrated))
+          if python3 or type(_x) == unicode:
+            _x = _x.encode('utf-8')
+            length = len(_x)
+          buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+          _x = _v2.lastChange
+          buff.write(_get_struct_I().pack(_x))
+          length = len(_v2.metrics)
+          buff.write(_struct_I.pack(length))
+          for val4 in _v2.metrics:
+            _x = val4.name
+            length = len(_x)
+            if python3 or type(_x) == unicode:
+              _x = _x.encode('utf-8')
+              length = len(_x)
+            buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+            _x = val4.value
+            length = len(_x)
+            if python3 or type(_x) == unicode:
+              _x = _x.encode('utf-8')
+              length = len(_x)
+            buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+          length = len(val2.sensors)
+          buff.write(_struct_I.pack(length))
+          for val3 in val2.sensors:
+            _x = val3.sensor_id
+            length = len(_x)
+            if python3 or type(_x) == unicode:
+              _x = _x.encode('utf-8')
+              length = len(_x)
+            buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+            _x = val3.model
+            length = len(_x)
+            if python3 or type(_x) == unicode:
+              _x = _x.encode('utf-8')
+              length = len(_x)
+            buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+            _x = val3.type
+            buff.write(_get_struct_I().pack(_x))
+            _v3 = val3.pose
+            _v4 = _v3.position
+            _x = _v4
+            buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
+            _v5 = _v3.orientation
+            _x = _v5
+            buff.write(_get_struct_4d().pack(_x.x, _x.y, _x.z, _x.w))
+            _x = val3
+            buff.write(_get_struct_f3IfB().pack(_x.azimuth, _x.image_width, _x.image_height, _x.frame_rate, _x.power, _x.calibrated))
+            _v6 = val3.state
+            _x = _v6
+            buff.write(_get_struct_3I().pack(_x.id, _x.state, _x.status))
+            _x = _v6.description
+            length = len(_x)
+            if python3 or type(_x) == unicode:
+              _x = _x.encode('utf-8')
+              length = len(_x)
+            buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+            _x = _v6.lastChange
+            buff.write(_get_struct_I().pack(_x))
+            length = len(_v6.metrics)
+            buff.write(_struct_I.pack(length))
+            for val5 in _v6.metrics:
+              _x = val5.name
+              length = len(_x)
+              if python3 or type(_x) == unicode:
+                _x = _x.encode('utf-8')
+                length = len(_x)
+              buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+              _x = val5.value
+              length = len(_x)
+              if python3 or type(_x) == unicode:
+                _x = _x.encode('utf-8')
+                length = len(_x)
+              buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+            _v7 = val3.imu
+            _x = _v7.heading
+            buff.write(_get_struct_f().pack(_x))
+            _x = _v7.device_id
+            length = len(_x)
+            if python3 or type(_x) == unicode:
+              _x = _x.encode('utf-8')
+              length = len(_x)
+            buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+            _v8 = _v7.imu
+            _v9 = _v8.header
+            _x = _v9.seq
+            buff.write(_get_struct_I().pack(_x))
+            _v10 = _v9.stamp
+            _x = _v10
+            buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
+            _x = _v9.frame_id
+            length = len(_x)
+            if python3 or type(_x) == unicode:
+              _x = _x.encode('utf-8')
+              length = len(_x)
+            buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+            _v11 = _v8.orientation
+            _x = _v11
+            buff.write(_get_struct_4d().pack(_x.x, _x.y, _x.z, _x.w))
+            buff.write(_get_struct_9d().pack(*_v8.orientation_covariance))
+            _v12 = _v8.angular_velocity
+            _x = _v12
+            buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
+            buff.write(_get_struct_9d().pack(*_v8.angular_velocity_covariance))
+            _v13 = _v8.linear_acceleration
+            _x = _v13
+            buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
+            buff.write(_get_struct_9d().pack(*_v8.linear_acceleration_covariance))
+            _v14 = _v7.magnetic_field
+            _x = _v14
+            buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
+            _x = _v7
+            buff.write(_get_struct_2fB().pack(_x.roll, _x.pitch, _x.deviceCalibrated))
     except struct.error as se: self._check_types(struct.error("%s: '%s' when writing '%s'" % (type(se), str(se), str(locals().get('_x', self)))))
     except TypeError as te: self._check_types(ValueError("%s: '%s' when writing '%s'" % (type(te), str(te), str(locals().get('_x', self)))))
 
   def deserialize(self, str):
     """
     unpack serialized message in str into this message instance
     :param str: byte array of serialized message, ``str``
     """
     if python3:
       codecs.lookup_error("rosmsg").msg_type = self._type
     try:
-      if self.sensors is None:
-        self.sensors = None
+      if self.status is None:
+        self.status = digitaleye_msgs.msg.DigitalEyeStatus()
       end = 0
+      _x = self
       start = end
-      end += 4
-      (self.system_id,) = _get_struct_I().unpack(str[start:end])
+      end += 16
+      (_x.status.started, _x.status.digitaleye.id, _x.status.digitaleye.state, _x.status.digitaleye.status,) = _get_struct_4I().unpack(str[start:end])
       start = end
       end += 4
       (length,) = _struct_I.unpack(str[start:end])
       start = end
       end += length
       if python3:
-        self.ip_address = str[start:end].decode('utf-8', 'rosmsg')
+        self.status.digitaleye.description = str[start:end].decode('utf-8', 'rosmsg')
       else:
-        self.ip_address = str[start:end]
+        self.status.digitaleye.description = str[start:end]
       start = end
       end += 4
-      (self.port,) = _get_struct_I().unpack(str[start:end])
+      (self.status.digitaleye.lastChange,) = _get_struct_I().unpack(str[start:end])
       start = end
       end += 4
       (length,) = _struct_I.unpack(str[start:end])
-      self.sensors = []
+      self.status.digitaleye.metrics = []
       for i in range(0, length):
-        val1 = digitaleye_msgs.msg.Sensor()
+        val1 = digitaleye_msgs.msg.Metric()
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
         start = end
         end += length
         if python3:
-          val1.sensor_id = str[start:end].decode('utf-8', 'rosmsg')
+          val1.name = str[start:end].decode('utf-8', 'rosmsg')
         else:
-          val1.sensor_id = str[start:end]
+          val1.name = str[start:end]
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
         start = end
         end += length
         if python3:
-          val1.model = str[start:end].decode('utf-8', 'rosmsg')
+          val1.value = str[start:end].decode('utf-8', 'rosmsg')
         else:
-          val1.model = str[start:end]
-        start = end
-        end += 4
-        (val1.type,) = _get_struct_I().unpack(str[start:end])
-        _v13 = val1.pose
-        _v14 = _v13.position
-        _x = _v14
-        start = end
-        end += 24
-        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        _v15 = _v13.orientation
+          val1.value = str[start:end]
+        self.status.digitaleye.metrics.append(val1)
+      start = end
+      end += 4
+      (length,) = _struct_I.unpack(str[start:end])
+      self.status.subsystems = []
+      for i in range(0, length):
+        val1 = digitaleye_msgs.msg.SystemState()
+        _v15 = val1.system
         _x = _v15
         start = end
-        end += 32
-        (_x.x, _x.y, _x.z, _x.w,) = _get_struct_4d().unpack(str[start:end])
-        _x = val1
-        start = end
-        end += 21
-        (_x.azimuth, _x.image_width, _x.image_height, _x.frame_rate, _x.power, _x.calibrated,) = _get_struct_f3IfB().unpack(str[start:end])
-        val1.calibrated = bool(val1.calibrated)
-        _v16 = val1.state
-        _x = _v16
-        start = end
         end += 12
         (_x.id, _x.state, _x.status,) = _get_struct_3I().unpack(str[start:end])
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
         start = end
         end += length
         if python3:
-          _v16.description = str[start:end].decode('utf-8', 'rosmsg')
+          _v15.description = str[start:end].decode('utf-8', 'rosmsg')
         else:
-          _v16.description = str[start:end]
+          _v15.description = str[start:end]
         start = end
         end += 4
-        (_v16.lastChange,) = _get_struct_I().unpack(str[start:end])
+        (_v15.lastChange,) = _get_struct_I().unpack(str[start:end])
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
-        _v16.metrics = []
+        _v15.metrics = []
         for i in range(0, length):
           val3 = digitaleye_msgs.msg.Metric()
           start = end
           end += 4
           (length,) = _struct_I.unpack(str[start:end])
           start = end
           end += length
@@ -472,289 +642,486 @@
           (length,) = _struct_I.unpack(str[start:end])
           start = end
           end += length
           if python3:
             val3.value = str[start:end].decode('utf-8', 'rosmsg')
           else:
             val3.value = str[start:end]
-          _v16.metrics.append(val3)
-        _v17 = val1.imu
-        start = end
-        end += 4
-        (_v17.heading,) = _get_struct_f().unpack(str[start:end])
+          _v15.metrics.append(val3)
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
-        start = end
-        end += length
-        if python3:
-          _v17.device_id = str[start:end].decode('utf-8', 'rosmsg')
-        else:
-          _v17.device_id = str[start:end]
-        _v18 = _v17.imu
-        _v19 = _v18.header
-        start = end
-        end += 4
-        (_v19.seq,) = _get_struct_I().unpack(str[start:end])
-        _v20 = _v19.stamp
-        _x = _v20
-        start = end
-        end += 8
-        (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
-        start = end
-        end += 4
-        (length,) = _struct_I.unpack(str[start:end])
-        start = end
-        end += length
-        if python3:
-          _v19.frame_id = str[start:end].decode('utf-8', 'rosmsg')
-        else:
-          _v19.frame_id = str[start:end]
-        _v21 = _v18.orientation
-        _x = _v21
-        start = end
-        end += 32
-        (_x.x, _x.y, _x.z, _x.w,) = _get_struct_4d().unpack(str[start:end])
-        start = end
-        end += 72
-        _v18.orientation_covariance = _get_struct_9d().unpack(str[start:end])
-        _v22 = _v18.angular_velocity
-        _x = _v22
-        start = end
-        end += 24
-        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        start = end
-        end += 72
-        _v18.angular_velocity_covariance = _get_struct_9d().unpack(str[start:end])
-        _v23 = _v18.linear_acceleration
-        _x = _v23
-        start = end
-        end += 24
-        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        start = end
-        end += 72
-        _v18.linear_acceleration_covariance = _get_struct_9d().unpack(str[start:end])
-        _v24 = _v17.magnetic_field
-        _x = _v24
-        start = end
-        end += 24
-        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        _x = _v17
-        start = end
-        end += 9
-        (_x.roll, _x.pitch, _x.deviceCalibrated,) = _get_struct_2fB().unpack(str[start:end])
-        _v17.deviceCalibrated = bool(_v17.deviceCalibrated)
-        self.sensors.append(val1)
+        val1.components = []
+        for i in range(0, length):
+          val2 = digitaleye_msgs.msg.ComponentState()
+          _v16 = val2.component
+          _x = _v16
+          start = end
+          end += 12
+          (_x.id, _x.state, _x.status,) = _get_struct_3I().unpack(str[start:end])
+          start = end
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          start = end
+          end += length
+          if python3:
+            _v16.description = str[start:end].decode('utf-8', 'rosmsg')
+          else:
+            _v16.description = str[start:end]
+          start = end
+          end += 4
+          (_v16.lastChange,) = _get_struct_I().unpack(str[start:end])
+          start = end
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          _v16.metrics = []
+          for i in range(0, length):
+            val4 = digitaleye_msgs.msg.Metric()
+            start = end
+            end += 4
+            (length,) = _struct_I.unpack(str[start:end])
+            start = end
+            end += length
+            if python3:
+              val4.name = str[start:end].decode('utf-8', 'rosmsg')
+            else:
+              val4.name = str[start:end]
+            start = end
+            end += 4
+            (length,) = _struct_I.unpack(str[start:end])
+            start = end
+            end += length
+            if python3:
+              val4.value = str[start:end].decode('utf-8', 'rosmsg')
+            else:
+              val4.value = str[start:end]
+            _v16.metrics.append(val4)
+          start = end
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          val2.sensors = []
+          for i in range(0, length):
+            val3 = digitaleye_msgs.msg.Sensor()
+            start = end
+            end += 4
+            (length,) = _struct_I.unpack(str[start:end])
+            start = end
+            end += length
+            if python3:
+              val3.sensor_id = str[start:end].decode('utf-8', 'rosmsg')
+            else:
+              val3.sensor_id = str[start:end]
+            start = end
+            end += 4
+            (length,) = _struct_I.unpack(str[start:end])
+            start = end
+            end += length
+            if python3:
+              val3.model = str[start:end].decode('utf-8', 'rosmsg')
+            else:
+              val3.model = str[start:end]
+            start = end
+            end += 4
+            (val3.type,) = _get_struct_I().unpack(str[start:end])
+            _v17 = val3.pose
+            _v18 = _v17.position
+            _x = _v18
+            start = end
+            end += 24
+            (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
+            _v19 = _v17.orientation
+            _x = _v19
+            start = end
+            end += 32
+            (_x.x, _x.y, _x.z, _x.w,) = _get_struct_4d().unpack(str[start:end])
+            _x = val3
+            start = end
+            end += 21
+            (_x.azimuth, _x.image_width, _x.image_height, _x.frame_rate, _x.power, _x.calibrated,) = _get_struct_f3IfB().unpack(str[start:end])
+            val3.calibrated = bool(val3.calibrated)
+            _v20 = val3.state
+            _x = _v20
+            start = end
+            end += 12
+            (_x.id, _x.state, _x.status,) = _get_struct_3I().unpack(str[start:end])
+            start = end
+            end += 4
+            (length,) = _struct_I.unpack(str[start:end])
+            start = end
+            end += length
+            if python3:
+              _v20.description = str[start:end].decode('utf-8', 'rosmsg')
+            else:
+              _v20.description = str[start:end]
+            start = end
+            end += 4
+            (_v20.lastChange,) = _get_struct_I().unpack(str[start:end])
+            start = end
+            end += 4
+            (length,) = _struct_I.unpack(str[start:end])
+            _v20.metrics = []
+            for i in range(0, length):
+              val5 = digitaleye_msgs.msg.Metric()
+              start = end
+              end += 4
+              (length,) = _struct_I.unpack(str[start:end])
+              start = end
+              end += length
+              if python3:
+                val5.name = str[start:end].decode('utf-8', 'rosmsg')
+              else:
+                val5.name = str[start:end]
+              start = end
+              end += 4
+              (length,) = _struct_I.unpack(str[start:end])
+              start = end
+              end += length
+              if python3:
+                val5.value = str[start:end].decode('utf-8', 'rosmsg')
+              else:
+                val5.value = str[start:end]
+              _v20.metrics.append(val5)
+            _v21 = val3.imu
+            start = end
+            end += 4
+            (_v21.heading,) = _get_struct_f().unpack(str[start:end])
+            start = end
+            end += 4
+            (length,) = _struct_I.unpack(str[start:end])
+            start = end
+            end += length
+            if python3:
+              _v21.device_id = str[start:end].decode('utf-8', 'rosmsg')
+            else:
+              _v21.device_id = str[start:end]
+            _v22 = _v21.imu
+            _v23 = _v22.header
+            start = end
+            end += 4
+            (_v23.seq,) = _get_struct_I().unpack(str[start:end])
+            _v24 = _v23.stamp
+            _x = _v24
+            start = end
+            end += 8
+            (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
+            start = end
+            end += 4
+            (length,) = _struct_I.unpack(str[start:end])
+            start = end
+            end += length
+            if python3:
+              _v23.frame_id = str[start:end].decode('utf-8', 'rosmsg')
+            else:
+              _v23.frame_id = str[start:end]
+            _v25 = _v22.orientation
+            _x = _v25
+            start = end
+            end += 32
+            (_x.x, _x.y, _x.z, _x.w,) = _get_struct_4d().unpack(str[start:end])
+            start = end
+            end += 72
+            _v22.orientation_covariance = _get_struct_9d().unpack(str[start:end])
+            _v26 = _v22.angular_velocity
+            _x = _v26
+            start = end
+            end += 24
+            (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
+            start = end
+            end += 72
+            _v22.angular_velocity_covariance = _get_struct_9d().unpack(str[start:end])
+            _v27 = _v22.linear_acceleration
+            _x = _v27
+            start = end
+            end += 24
+            (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
+            start = end
+            end += 72
+            _v22.linear_acceleration_covariance = _get_struct_9d().unpack(str[start:end])
+            _v28 = _v21.magnetic_field
+            _x = _v28
+            start = end
+            end += 24
+            (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
+            _x = _v21
+            start = end
+            end += 9
+            (_x.roll, _x.pitch, _x.deviceCalibrated,) = _get_struct_2fB().unpack(str[start:end])
+            _v21.deviceCalibrated = bool(_v21.deviceCalibrated)
+            val2.sensors.append(val3)
+          val1.components.append(val2)
+        self.status.subsystems.append(val1)
       return self
     except struct.error as e:
       raise genpy.DeserializationError(e)  # most likely buffer underfill
 
 
   def serialize_numpy(self, buff, numpy):
     """
     serialize message with numpy array types into buffer
     :param buff: buffer, ``StringIO``
     :param numpy: numpy python module
     """
     try:
-      _x = self.system_id
-      buff.write(_get_struct_I().pack(_x))
-      _x = self.ip_address
+      _x = self
+      buff.write(_get_struct_4I().pack(_x.status.started, _x.status.digitaleye.id, _x.status.digitaleye.state, _x.status.digitaleye.status))
+      _x = self.status.digitaleye.description
       length = len(_x)
       if python3 or type(_x) == unicode:
         _x = _x.encode('utf-8')
         length = len(_x)
       buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-      _x = self.port
+      _x = self.status.digitaleye.lastChange
       buff.write(_get_struct_I().pack(_x))
-      length = len(self.sensors)
+      length = len(self.status.digitaleye.metrics)
       buff.write(_struct_I.pack(length))
-      for val1 in self.sensors:
-        _x = val1.sensor_id
+      for val1 in self.status.digitaleye.metrics:
+        _x = val1.name
         length = len(_x)
         if python3 or type(_x) == unicode:
           _x = _x.encode('utf-8')
           length = len(_x)
         buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = val1.model
+        _x = val1.value
         length = len(_x)
         if python3 or type(_x) == unicode:
           _x = _x.encode('utf-8')
           length = len(_x)
         buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = val1.type
-        buff.write(_get_struct_I().pack(_x))
-        _v25 = val1.pose
-        _v26 = _v25.position
-        _x = _v26
-        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        _v27 = _v25.orientation
-        _x = _v27
-        buff.write(_get_struct_4d().pack(_x.x, _x.y, _x.z, _x.w))
-        _x = val1
-        buff.write(_get_struct_f3IfB().pack(_x.azimuth, _x.image_width, _x.image_height, _x.frame_rate, _x.power, _x.calibrated))
-        _v28 = val1.state
-        _x = _v28
+      length = len(self.status.subsystems)
+      buff.write(_struct_I.pack(length))
+      for val1 in self.status.subsystems:
+        _v29 = val1.system
+        _x = _v29
         buff.write(_get_struct_3I().pack(_x.id, _x.state, _x.status))
-        _x = _v28.description
+        _x = _v29.description
         length = len(_x)
         if python3 or type(_x) == unicode:
           _x = _x.encode('utf-8')
           length = len(_x)
         buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = _v28.lastChange
+        _x = _v29.lastChange
         buff.write(_get_struct_I().pack(_x))
-        length = len(_v28.metrics)
+        length = len(_v29.metrics)
         buff.write(_struct_I.pack(length))
-        for val3 in _v28.metrics:
+        for val3 in _v29.metrics:
           _x = val3.name
           length = len(_x)
           if python3 or type(_x) == unicode:
             _x = _x.encode('utf-8')
             length = len(_x)
           buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
           _x = val3.value
           length = len(_x)
           if python3 or type(_x) == unicode:
             _x = _x.encode('utf-8')
             length = len(_x)
           buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _v29 = val1.imu
-        _x = _v29.heading
-        buff.write(_get_struct_f().pack(_x))
-        _x = _v29.device_id
-        length = len(_x)
-        if python3 or type(_x) == unicode:
-          _x = _x.encode('utf-8')
-          length = len(_x)
-        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _v30 = _v29.imu
-        _v31 = _v30.header
-        _x = _v31.seq
-        buff.write(_get_struct_I().pack(_x))
-        _v32 = _v31.stamp
-        _x = _v32
-        buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
-        _x = _v31.frame_id
-        length = len(_x)
-        if python3 or type(_x) == unicode:
-          _x = _x.encode('utf-8')
+        length = len(val1.components)
+        buff.write(_struct_I.pack(length))
+        for val2 in val1.components:
+          _v30 = val2.component
+          _x = _v30
+          buff.write(_get_struct_3I().pack(_x.id, _x.state, _x.status))
+          _x = _v30.description
           length = len(_x)
-        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _v33 = _v30.orientation
-        _x = _v33
-        buff.write(_get_struct_4d().pack(_x.x, _x.y, _x.z, _x.w))
-        buff.write(_v30.orientation_covariance.tostring())
-        _v34 = _v30.angular_velocity
-        _x = _v34
-        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        buff.write(_v30.angular_velocity_covariance.tostring())
-        _v35 = _v30.linear_acceleration
-        _x = _v35
-        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        buff.write(_v30.linear_acceleration_covariance.tostring())
-        _v36 = _v29.magnetic_field
-        _x = _v36
-        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        _x = _v29
-        buff.write(_get_struct_2fB().pack(_x.roll, _x.pitch, _x.deviceCalibrated))
+          if python3 or type(_x) == unicode:
+            _x = _x.encode('utf-8')
+            length = len(_x)
+          buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+          _x = _v30.lastChange
+          buff.write(_get_struct_I().pack(_x))
+          length = len(_v30.metrics)
+          buff.write(_struct_I.pack(length))
+          for val4 in _v30.metrics:
+            _x = val4.name
+            length = len(_x)
+            if python3 or type(_x) == unicode:
+              _x = _x.encode('utf-8')
+              length = len(_x)
+            buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+            _x = val4.value
+            length = len(_x)
+            if python3 or type(_x) == unicode:
+              _x = _x.encode('utf-8')
+              length = len(_x)
+            buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+          length = len(val2.sensors)
+          buff.write(_struct_I.pack(length))
+          for val3 in val2.sensors:
+            _x = val3.sensor_id
+            length = len(_x)
+            if python3 or type(_x) == unicode:
+              _x = _x.encode('utf-8')
+              length = len(_x)
+            buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+            _x = val3.model
+            length = len(_x)
+            if python3 or type(_x) == unicode:
+              _x = _x.encode('utf-8')
+              length = len(_x)
+            buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+            _x = val3.type
+            buff.write(_get_struct_I().pack(_x))
+            _v31 = val3.pose
+            _v32 = _v31.position
+            _x = _v32
+            buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
+            _v33 = _v31.orientation
+            _x = _v33
+            buff.write(_get_struct_4d().pack(_x.x, _x.y, _x.z, _x.w))
+            _x = val3
+            buff.write(_get_struct_f3IfB().pack(_x.azimuth, _x.image_width, _x.image_height, _x.frame_rate, _x.power, _x.calibrated))
+            _v34 = val3.state
+            _x = _v34
+            buff.write(_get_struct_3I().pack(_x.id, _x.state, _x.status))
+            _x = _v34.description
+            length = len(_x)
+            if python3 or type(_x) == unicode:
+              _x = _x.encode('utf-8')
+              length = len(_x)
+            buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+            _x = _v34.lastChange
+            buff.write(_get_struct_I().pack(_x))
+            length = len(_v34.metrics)
+            buff.write(_struct_I.pack(length))
+            for val5 in _v34.metrics:
+              _x = val5.name
+              length = len(_x)
+              if python3 or type(_x) == unicode:
+                _x = _x.encode('utf-8')
+                length = len(_x)
+              buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+              _x = val5.value
+              length = len(_x)
+              if python3 or type(_x) == unicode:
+                _x = _x.encode('utf-8')
+                length = len(_x)
+              buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+            _v35 = val3.imu
+            _x = _v35.heading
+            buff.write(_get_struct_f().pack(_x))
+            _x = _v35.device_id
+            length = len(_x)
+            if python3 or type(_x) == unicode:
+              _x = _x.encode('utf-8')
+              length = len(_x)
+            buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+            _v36 = _v35.imu
+            _v37 = _v36.header
+            _x = _v37.seq
+            buff.write(_get_struct_I().pack(_x))
+            _v38 = _v37.stamp
+            _x = _v38
+            buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
+            _x = _v37.frame_id
+            length = len(_x)
+            if python3 or type(_x) == unicode:
+              _x = _x.encode('utf-8')
+              length = len(_x)
+            buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+            _v39 = _v36.orientation
+            _x = _v39
+            buff.write(_get_struct_4d().pack(_x.x, _x.y, _x.z, _x.w))
+            buff.write(_v36.orientation_covariance.tostring())
+            _v40 = _v36.angular_velocity
+            _x = _v40
+            buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
+            buff.write(_v36.angular_velocity_covariance.tostring())
+            _v41 = _v36.linear_acceleration
+            _x = _v41
+            buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
+            buff.write(_v36.linear_acceleration_covariance.tostring())
+            _v42 = _v35.magnetic_field
+            _x = _v42
+            buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
+            _x = _v35
+            buff.write(_get_struct_2fB().pack(_x.roll, _x.pitch, _x.deviceCalibrated))
     except struct.error as se: self._check_types(struct.error("%s: '%s' when writing '%s'" % (type(se), str(se), str(locals().get('_x', self)))))
     except TypeError as te: self._check_types(ValueError("%s: '%s' when writing '%s'" % (type(te), str(te), str(locals().get('_x', self)))))
 
   def deserialize_numpy(self, str, numpy):
     """
     unpack serialized message in str into this message instance using numpy for array types
     :param str: byte array of serialized message, ``str``
     :param numpy: numpy python module
     """
     if python3:
       codecs.lookup_error("rosmsg").msg_type = self._type
     try:
-      if self.sensors is None:
-        self.sensors = None
+      if self.status is None:
+        self.status = digitaleye_msgs.msg.DigitalEyeStatus()
       end = 0
+      _x = self
       start = end
-      end += 4
-      (self.system_id,) = _get_struct_I().unpack(str[start:end])
+      end += 16
+      (_x.status.started, _x.status.digitaleye.id, _x.status.digitaleye.state, _x.status.digitaleye.status,) = _get_struct_4I().unpack(str[start:end])
       start = end
       end += 4
       (length,) = _struct_I.unpack(str[start:end])
       start = end
       end += length
       if python3:
-        self.ip_address = str[start:end].decode('utf-8', 'rosmsg')
+        self.status.digitaleye.description = str[start:end].decode('utf-8', 'rosmsg')
       else:
-        self.ip_address = str[start:end]
+        self.status.digitaleye.description = str[start:end]
       start = end
       end += 4
-      (self.port,) = _get_struct_I().unpack(str[start:end])
+      (self.status.digitaleye.lastChange,) = _get_struct_I().unpack(str[start:end])
       start = end
       end += 4
       (length,) = _struct_I.unpack(str[start:end])
-      self.sensors = []
+      self.status.digitaleye.metrics = []
       for i in range(0, length):
-        val1 = digitaleye_msgs.msg.Sensor()
+        val1 = digitaleye_msgs.msg.Metric()
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
         start = end
         end += length
         if python3:
-          val1.sensor_id = str[start:end].decode('utf-8', 'rosmsg')
+          val1.name = str[start:end].decode('utf-8', 'rosmsg')
         else:
-          val1.sensor_id = str[start:end]
+          val1.name = str[start:end]
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
         start = end
         end += length
         if python3:
-          val1.model = str[start:end].decode('utf-8', 'rosmsg')
+          val1.value = str[start:end].decode('utf-8', 'rosmsg')
         else:
-          val1.model = str[start:end]
-        start = end
-        end += 4
-        (val1.type,) = _get_struct_I().unpack(str[start:end])
-        _v37 = val1.pose
-        _v38 = _v37.position
-        _x = _v38
-        start = end
-        end += 24
-        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        _v39 = _v37.orientation
-        _x = _v39
-        start = end
-        end += 32
-        (_x.x, _x.y, _x.z, _x.w,) = _get_struct_4d().unpack(str[start:end])
-        _x = val1
-        start = end
-        end += 21
-        (_x.azimuth, _x.image_width, _x.image_height, _x.frame_rate, _x.power, _x.calibrated,) = _get_struct_f3IfB().unpack(str[start:end])
-        val1.calibrated = bool(val1.calibrated)
-        _v40 = val1.state
-        _x = _v40
+          val1.value = str[start:end]
+        self.status.digitaleye.metrics.append(val1)
+      start = end
+      end += 4
+      (length,) = _struct_I.unpack(str[start:end])
+      self.status.subsystems = []
+      for i in range(0, length):
+        val1 = digitaleye_msgs.msg.SystemState()
+        _v43 = val1.system
+        _x = _v43
         start = end
         end += 12
         (_x.id, _x.state, _x.status,) = _get_struct_3I().unpack(str[start:end])
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
         start = end
         end += length
         if python3:
-          _v40.description = str[start:end].decode('utf-8', 'rosmsg')
+          _v43.description = str[start:end].decode('utf-8', 'rosmsg')
         else:
-          _v40.description = str[start:end]
+          _v43.description = str[start:end]
         start = end
         end += 4
-        (_v40.lastChange,) = _get_struct_I().unpack(str[start:end])
+        (_v43.lastChange,) = _get_struct_I().unpack(str[start:end])
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
-        _v40.metrics = []
+        _v43.metrics = []
         for i in range(0, length):
           val3 = digitaleye_msgs.msg.Metric()
           start = end
           end += 4
           (length,) = _struct_I.unpack(str[start:end])
           start = end
           end += length
@@ -767,82 +1134,217 @@
           (length,) = _struct_I.unpack(str[start:end])
           start = end
           end += length
           if python3:
             val3.value = str[start:end].decode('utf-8', 'rosmsg')
           else:
             val3.value = str[start:end]
-          _v40.metrics.append(val3)
-        _v41 = val1.imu
-        start = end
-        end += 4
-        (_v41.heading,) = _get_struct_f().unpack(str[start:end])
+          _v43.metrics.append(val3)
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
-        start = end
-        end += length
-        if python3:
-          _v41.device_id = str[start:end].decode('utf-8', 'rosmsg')
-        else:
-          _v41.device_id = str[start:end]
-        _v42 = _v41.imu
-        _v43 = _v42.header
-        start = end
-        end += 4
-        (_v43.seq,) = _get_struct_I().unpack(str[start:end])
-        _v44 = _v43.stamp
-        _x = _v44
-        start = end
-        end += 8
-        (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
-        start = end
-        end += 4
-        (length,) = _struct_I.unpack(str[start:end])
-        start = end
-        end += length
-        if python3:
-          _v43.frame_id = str[start:end].decode('utf-8', 'rosmsg')
-        else:
-          _v43.frame_id = str[start:end]
-        _v45 = _v42.orientation
-        _x = _v45
-        start = end
-        end += 32
-        (_x.x, _x.y, _x.z, _x.w,) = _get_struct_4d().unpack(str[start:end])
-        start = end
-        end += 72
-        _v42.orientation_covariance = numpy.frombuffer(str[start:end], dtype=numpy.float64, count=9)
-        _v46 = _v42.angular_velocity
-        _x = _v46
-        start = end
-        end += 24
-        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        start = end
-        end += 72
-        _v42.angular_velocity_covariance = numpy.frombuffer(str[start:end], dtype=numpy.float64, count=9)
-        _v47 = _v42.linear_acceleration
-        _x = _v47
-        start = end
-        end += 24
-        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        start = end
-        end += 72
-        _v42.linear_acceleration_covariance = numpy.frombuffer(str[start:end], dtype=numpy.float64, count=9)
-        _v48 = _v41.magnetic_field
-        _x = _v48
-        start = end
-        end += 24
-        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        _x = _v41
-        start = end
-        end += 9
-        (_x.roll, _x.pitch, _x.deviceCalibrated,) = _get_struct_2fB().unpack(str[start:end])
-        _v41.deviceCalibrated = bool(_v41.deviceCalibrated)
-        self.sensors.append(val1)
+        val1.components = []
+        for i in range(0, length):
+          val2 = digitaleye_msgs.msg.ComponentState()
+          _v44 = val2.component
+          _x = _v44
+          start = end
+          end += 12
+          (_x.id, _x.state, _x.status,) = _get_struct_3I().unpack(str[start:end])
+          start = end
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          start = end
+          end += length
+          if python3:
+            _v44.description = str[start:end].decode('utf-8', 'rosmsg')
+          else:
+            _v44.description = str[start:end]
+          start = end
+          end += 4
+          (_v44.lastChange,) = _get_struct_I().unpack(str[start:end])
+          start = end
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          _v44.metrics = []
+          for i in range(0, length):
+            val4 = digitaleye_msgs.msg.Metric()
+            start = end
+            end += 4
+            (length,) = _struct_I.unpack(str[start:end])
+            start = end
+            end += length
+            if python3:
+              val4.name = str[start:end].decode('utf-8', 'rosmsg')
+            else:
+              val4.name = str[start:end]
+            start = end
+            end += 4
+            (length,) = _struct_I.unpack(str[start:end])
+            start = end
+            end += length
+            if python3:
+              val4.value = str[start:end].decode('utf-8', 'rosmsg')
+            else:
+              val4.value = str[start:end]
+            _v44.metrics.append(val4)
+          start = end
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          val2.sensors = []
+          for i in range(0, length):
+            val3 = digitaleye_msgs.msg.Sensor()
+            start = end
+            end += 4
+            (length,) = _struct_I.unpack(str[start:end])
+            start = end
+            end += length
+            if python3:
+              val3.sensor_id = str[start:end].decode('utf-8', 'rosmsg')
+            else:
+              val3.sensor_id = str[start:end]
+            start = end
+            end += 4
+            (length,) = _struct_I.unpack(str[start:end])
+            start = end
+            end += length
+            if python3:
+              val3.model = str[start:end].decode('utf-8', 'rosmsg')
+            else:
+              val3.model = str[start:end]
+            start = end
+            end += 4
+            (val3.type,) = _get_struct_I().unpack(str[start:end])
+            _v45 = val3.pose
+            _v46 = _v45.position
+            _x = _v46
+            start = end
+            end += 24
+            (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
+            _v47 = _v45.orientation
+            _x = _v47
+            start = end
+            end += 32
+            (_x.x, _x.y, _x.z, _x.w,) = _get_struct_4d().unpack(str[start:end])
+            _x = val3
+            start = end
+            end += 21
+            (_x.azimuth, _x.image_width, _x.image_height, _x.frame_rate, _x.power, _x.calibrated,) = _get_struct_f3IfB().unpack(str[start:end])
+            val3.calibrated = bool(val3.calibrated)
+            _v48 = val3.state
+            _x = _v48
+            start = end
+            end += 12
+            (_x.id, _x.state, _x.status,) = _get_struct_3I().unpack(str[start:end])
+            start = end
+            end += 4
+            (length,) = _struct_I.unpack(str[start:end])
+            start = end
+            end += length
+            if python3:
+              _v48.description = str[start:end].decode('utf-8', 'rosmsg')
+            else:
+              _v48.description = str[start:end]
+            start = end
+            end += 4
+            (_v48.lastChange,) = _get_struct_I().unpack(str[start:end])
+            start = end
+            end += 4
+            (length,) = _struct_I.unpack(str[start:end])
+            _v48.metrics = []
+            for i in range(0, length):
+              val5 = digitaleye_msgs.msg.Metric()
+              start = end
+              end += 4
+              (length,) = _struct_I.unpack(str[start:end])
+              start = end
+              end += length
+              if python3:
+                val5.name = str[start:end].decode('utf-8', 'rosmsg')
+              else:
+                val5.name = str[start:end]
+              start = end
+              end += 4
+              (length,) = _struct_I.unpack(str[start:end])
+              start = end
+              end += length
+              if python3:
+                val5.value = str[start:end].decode('utf-8', 'rosmsg')
+              else:
+                val5.value = str[start:end]
+              _v48.metrics.append(val5)
+            _v49 = val3.imu
+            start = end
+            end += 4
+            (_v49.heading,) = _get_struct_f().unpack(str[start:end])
+            start = end
+            end += 4
+            (length,) = _struct_I.unpack(str[start:end])
+            start = end
+            end += length
+            if python3:
+              _v49.device_id = str[start:end].decode('utf-8', 'rosmsg')
+            else:
+              _v49.device_id = str[start:end]
+            _v50 = _v49.imu
+            _v51 = _v50.header
+            start = end
+            end += 4
+            (_v51.seq,) = _get_struct_I().unpack(str[start:end])
+            _v52 = _v51.stamp
+            _x = _v52
+            start = end
+            end += 8
+            (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
+            start = end
+            end += 4
+            (length,) = _struct_I.unpack(str[start:end])
+            start = end
+            end += length
+            if python3:
+              _v51.frame_id = str[start:end].decode('utf-8', 'rosmsg')
+            else:
+              _v51.frame_id = str[start:end]
+            _v53 = _v50.orientation
+            _x = _v53
+            start = end
+            end += 32
+            (_x.x, _x.y, _x.z, _x.w,) = _get_struct_4d().unpack(str[start:end])
+            start = end
+            end += 72
+            _v50.orientation_covariance = numpy.frombuffer(str[start:end], dtype=numpy.float64, count=9)
+            _v54 = _v50.angular_velocity
+            _x = _v54
+            start = end
+            end += 24
+            (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
+            start = end
+            end += 72
+            _v50.angular_velocity_covariance = numpy.frombuffer(str[start:end], dtype=numpy.float64, count=9)
+            _v55 = _v50.linear_acceleration
+            _x = _v55
+            start = end
+            end += 24
+            (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
+            start = end
+            end += 72
+            _v50.linear_acceleration_covariance = numpy.frombuffer(str[start:end], dtype=numpy.float64, count=9)
+            _v56 = _v49.magnetic_field
+            _x = _v56
+            start = end
+            end += 24
+            (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
+            _x = _v49
+            start = end
+            end += 9
+            (_x.roll, _x.pitch, _x.deviceCalibrated,) = _get_struct_2fB().unpack(str[start:end])
+            _v49.deviceCalibrated = bool(_v49.deviceCalibrated)
+            val2.sensors.append(val3)
+          val1.components.append(val2)
+        self.status.subsystems.append(val1)
       return self
     except struct.error as e:
       raise genpy.DeserializationError(e)  # most likely buffer underfill
 
 _struct_I = genpy.struct_I
 def _get_struct_I():
     global _struct_I
@@ -867,14 +1369,20 @@
     return _struct_3I
 _struct_3d = None
 def _get_struct_3d():
     global _struct_3d
     if _struct_3d is None:
         _struct_3d = struct.Struct("<3d")
     return _struct_3d
+_struct_4I = None
+def _get_struct_4I():
+    global _struct_4I
+    if _struct_4I is None:
+        _struct_4I = struct.Struct("<4I")
+    return _struct_4I
 _struct_4d = None
 def _get_struct_4d():
     global _struct_4d
     if _struct_4d is None:
         _struct_4d = struct.Struct("<4d")
     return _struct_4d
 _struct_9d = None
@@ -891,7 +1399,12 @@
     return _struct_f
 _struct_f3IfB = None
 def _get_struct_f3IfB():
     global _struct_f3IfB
     if _struct_f3IfB is None:
         _struct_f3IfB = struct.Struct("<f3IfB")
     return _struct_f3IfB
+class GetStatus(object):
+  _type          = 'digitaleye_msgs/GetStatus'
+  _md5sum = '3debe849e7d84e1c8a45738e73fc747e'
+  _request_class  = GetStatusRequest
+  _response_class = GetStatusResponse
```

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_SystemNotification.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_SystemNotification.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_SystemState.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetPoles.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,188 @@
 # This Python file uses the following encoding: utf-8
-"""autogenerated by genpy from digitaleye_msgs/SystemState.msg. Do not edit."""
+"""autogenerated by genpy from digitaleye_msgs/GetPolesRequest.msg. Do not edit."""
+import codecs
+import sys
+python3 = True if sys.hexversion > 0x03000000 else False
+import genpy
+import struct
+
+
+class GetPolesRequest(genpy.Message):
+  _md5sum = "d41d8cd98f00b204e9800998ecf8427e"
+  _type = "digitaleye_msgs/GetPolesRequest"
+  _has_header = False  # flag to mark the presence of a Header object
+  _full_text = """"""
+  __slots__ = []
+  _slot_types = []
+
+  def __init__(self, *args, **kwds):
+    """
+    Constructor. Any message fields that are implicitly/explicitly
+    set to None will be assigned a default value. The recommend
+    use is keyword arguments as this is more robust to future message
+    changes.  You cannot mix in-order arguments and keyword arguments.
+
+    The available fields are:
+       
+
+    :param args: complete set of field values, in .msg order
+    :param kwds: use keyword arguments corresponding to message field names
+    to set specific fields.
+    """
+    if args or kwds:
+      super(GetPolesRequest, self).__init__(*args, **kwds)
+
+  def _get_types(self):
+    """
+    internal API method
+    """
+    return self._slot_types
+
+  def serialize(self, buff):
+    """
+    serialize message into buffer
+    :param buff: buffer, ``StringIO``
+    """
+    try:
+      pass
+    except struct.error as se: self._check_types(struct.error("%s: '%s' when writing '%s'" % (type(se), str(se), str(locals().get('_x', self)))))
+    except TypeError as te: self._check_types(ValueError("%s: '%s' when writing '%s'" % (type(te), str(te), str(locals().get('_x', self)))))
+
+  def deserialize(self, str):
+    """
+    unpack serialized message in str into this message instance
+    :param str: byte array of serialized message, ``str``
+    """
+    if python3:
+      codecs.lookup_error("rosmsg").msg_type = self._type
+    try:
+      end = 0
+      return self
+    except struct.error as e:
+      raise genpy.DeserializationError(e)  # most likely buffer underfill
+
+
+  def serialize_numpy(self, buff, numpy):
+    """
+    serialize message with numpy array types into buffer
+    :param buff: buffer, ``StringIO``
+    :param numpy: numpy python module
+    """
+    try:
+      pass
+    except struct.error as se: self._check_types(struct.error("%s: '%s' when writing '%s'" % (type(se), str(se), str(locals().get('_x', self)))))
+    except TypeError as te: self._check_types(ValueError("%s: '%s' when writing '%s'" % (type(te), str(te), str(locals().get('_x', self)))))
+
+  def deserialize_numpy(self, str, numpy):
+    """
+    unpack serialized message in str into this message instance using numpy for array types
+    :param str: byte array of serialized message, ``str``
+    :param numpy: numpy python module
+    """
+    if python3:
+      codecs.lookup_error("rosmsg").msg_type = self._type
+    try:
+      end = 0
+      return self
+    except struct.error as e:
+      raise genpy.DeserializationError(e)  # most likely buffer underfill
+
+_struct_I = genpy.struct_I
+def _get_struct_I():
+    global _struct_I
+    return _struct_I
+# This Python file uses the following encoding: utf-8
+"""autogenerated by genpy from digitaleye_msgs/GetPolesResponse.msg. Do not edit."""
 import codecs
 import sys
 python3 = True if sys.hexversion > 0x03000000 else False
 import genpy
 import struct
 
 import digitaleye_msgs.msg
 import geometry_msgs.msg
 import sensor_msgs.msg
 import std_msgs.msg
 
-class SystemState(genpy.Message):
-  _md5sum = "f373ec9b3610db5e16911fbb76684b9c"
-  _type = "digitaleye_msgs/SystemState"
+class GetPolesResponse(genpy.Message):
+  _md5sum = "7495bec4b83825ae9001a24db3ee7d3f"
+  _type = "digitaleye_msgs/GetPolesResponse"
   _has_header = False  # flag to mark the presence of a Header object
-  _full_text = """# State of a system and its constituent subsystem(s)
+  _full_text = """# List of poles last detected by the DEMS
+digitaleye_msgs/Position position
+
+
+================================================================================
+MSG: digitaleye_msgs/Position
+# Position of all of the DigitalEye’s physical components
+
+# list of pole(s) in the current DigitalEye
+# configuration and their positions
+digitaleye_msgs/Pole[] poles
+
+================================================================================
+MSG: digitaleye_msgs/Pole
+# Description of the position and status of
+# a DigitalEye’s sensor pole
+
+# unique identifier of the pole being described
+uint32 id
+
+# pole’s IP address on the main subnet
+string ip_address
+
+# IP address of the MVC attached to the pole
+string mvc
+
+# MAC address of the iot locator attached to the pole
+string iot
+
+# unique identifier of the reference frame in which
+# the pole’s position is given
+uint32 position_frame
 
-# state of the system
-digitaleye_msgs/State system
+# coordinates of the pole within the specified
+# reference frame (either in meters or in order lat, long in degrees
+# and alt in meters (WGS84 ellipsoid or MSL)
+geometry_msgs/Point position
 
-# list of the state(s) of the system’s constituent component(s)
-digitaleye_msgs/ComponentState[] components
+# unique identifier of the reference frame in which
+# the pole’s orientation is given
+uint32 orientation_frame
+
+# direction the pole is facing within the specified
+# reference frame
+float32 orientation
+
+# distance of the pole’s RTK receiver above the ground (meters)
+float32 height
+
+# current state of the pole
+digitaleye_msgs/ComponentState state
+
+# Key/value pairs representing the currently active pole settings
+digitaleye_msgs/Metric[] settings
+
+================================================================================
+MSG: geometry_msgs/Point
+# This contains the position of a point in free space
+float64 x
+float64 y
+float64 z
+
+================================================================================
+MSG: digitaleye_msgs/ComponentState
+# State of a system component and its attached sensor(s)
+
+# state of the component
+digitaleye_msgs/State component
+
+# state(s) of the component’s attached sensor(s)
+digitaleye_msgs/Sensor[] sensors
 
 ================================================================================
 MSG: digitaleye_msgs/State
 # Details of a system’s status
 
 # unique identifier of the system
 # whose status is being reported
@@ -58,24 +215,14 @@
 # name of the performance indicator
 string name
 
 # value of the performance indicator
 string value
 
 ================================================================================
-MSG: digitaleye_msgs/ComponentState
-# State of a system component and its attached sensor(s)
-
-# state of the component
-digitaleye_msgs/State component
-
-# state(s) of the component’s attached sensor(s)
-digitaleye_msgs/Sensor[] sensors
-
-================================================================================
 MSG: digitaleye_msgs/Sensor
 # Description of a monitoring DigitalEye sensor
 # and its properties
 
 # unique identifier of the sensor
 # e.g. hardware serial number
 string sensor_id
@@ -119,21 +266,14 @@
 ================================================================================
 MSG: geometry_msgs/Pose
 # A representation of pose in free space, composed of position and orientation. 
 Point position
 Quaternion orientation
 
 ================================================================================
-MSG: geometry_msgs/Point
-# This contains the position of a point in free space
-float64 x
-float64 y
-float64 z
-
-================================================================================
 MSG: geometry_msgs/Quaternion
 # This represents an orientation in free space in quaternion form.
 
 float64 x
 float64 y
 float64 z
 float64 w
@@ -215,873 +355,956 @@
 # generic rigid transformation to a Vector3, tf2 will only apply the
 # rotation). If you want your data to be translatable too, use the
 # geometry_msgs/Point message instead.
 
 float64 x
 float64 y
 float64 z"""
-  __slots__ = ['system','components']
-  _slot_types = ['digitaleye_msgs/State','digitaleye_msgs/ComponentState[]']
+  __slots__ = ['position']
+  _slot_types = ['digitaleye_msgs/Position']
 
   def __init__(self, *args, **kwds):
     """
     Constructor. Any message fields that are implicitly/explicitly
     set to None will be assigned a default value. The recommend
     use is keyword arguments as this is more robust to future message
     changes.  You cannot mix in-order arguments and keyword arguments.
 
     The available fields are:
-       system,components
+       position
 
     :param args: complete set of field values, in .msg order
     :param kwds: use keyword arguments corresponding to message field names
     to set specific fields.
     """
     if args or kwds:
-      super(SystemState, self).__init__(*args, **kwds)
+      super(GetPolesResponse, self).__init__(*args, **kwds)
       # message fields cannot be None, assign default values for those that are
-      if self.system is None:
-        self.system = digitaleye_msgs.msg.State()
-      if self.components is None:
-        self.components = []
+      if self.position is None:
+        self.position = digitaleye_msgs.msg.Position()
     else:
-      self.system = digitaleye_msgs.msg.State()
-      self.components = []
+      self.position = digitaleye_msgs.msg.Position()
 
   def _get_types(self):
     """
     internal API method
     """
     return self._slot_types
 
   def serialize(self, buff):
     """
     serialize message into buffer
     :param buff: buffer, ``StringIO``
     """
     try:
-      _x = self
-      buff.write(_get_struct_3I().pack(_x.system.id, _x.system.state, _x.system.status))
-      _x = self.system.description
-      length = len(_x)
-      if python3 or type(_x) == unicode:
-        _x = _x.encode('utf-8')
-        length = len(_x)
-      buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-      _x = self.system.lastChange
-      buff.write(_get_struct_I().pack(_x))
-      length = len(self.system.metrics)
+      length = len(self.position.poles)
       buff.write(_struct_I.pack(length))
-      for val1 in self.system.metrics:
-        _x = val1.name
+      for val1 in self.position.poles:
+        _x = val1.id
+        buff.write(_get_struct_I().pack(_x))
+        _x = val1.ip_address
         length = len(_x)
         if python3 or type(_x) == unicode:
           _x = _x.encode('utf-8')
           length = len(_x)
         buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = val1.value
+        _x = val1.mvc
         length = len(_x)
         if python3 or type(_x) == unicode:
           _x = _x.encode('utf-8')
           length = len(_x)
         buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-      length = len(self.components)
-      buff.write(_struct_I.pack(length))
-      for val1 in self.components:
-        _v1 = val1.component
+        _x = val1.iot
+        length = len(_x)
+        if python3 or type(_x) == unicode:
+          _x = _x.encode('utf-8')
+          length = len(_x)
+        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+        _x = val1.position_frame
+        buff.write(_get_struct_I().pack(_x))
+        _v1 = val1.position
         _x = _v1
+        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
+        _x = val1
+        buff.write(_get_struct_I2f().pack(_x.orientation_frame, _x.orientation, _x.height))
+        _v2 = val1.state
+        _v3 = _v2.component
+        _x = _v3
         buff.write(_get_struct_3I().pack(_x.id, _x.state, _x.status))
-        _x = _v1.description
+        _x = _v3.description
         length = len(_x)
         if python3 or type(_x) == unicode:
           _x = _x.encode('utf-8')
           length = len(_x)
         buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = _v1.lastChange
+        _x = _v3.lastChange
         buff.write(_get_struct_I().pack(_x))
-        length = len(_v1.metrics)
+        length = len(_v3.metrics)
         buff.write(_struct_I.pack(length))
-        for val3 in _v1.metrics:
-          _x = val3.name
+        for val4 in _v3.metrics:
+          _x = val4.name
           length = len(_x)
           if python3 or type(_x) == unicode:
             _x = _x.encode('utf-8')
             length = len(_x)
           buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-          _x = val3.value
+          _x = val4.value
           length = len(_x)
           if python3 or type(_x) == unicode:
             _x = _x.encode('utf-8')
             length = len(_x)
           buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        length = len(val1.sensors)
+        length = len(_v2.sensors)
         buff.write(_struct_I.pack(length))
-        for val2 in val1.sensors:
-          _x = val2.sensor_id
+        for val3 in _v2.sensors:
+          _x = val3.sensor_id
           length = len(_x)
           if python3 or type(_x) == unicode:
             _x = _x.encode('utf-8')
             length = len(_x)
           buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-          _x = val2.model
+          _x = val3.model
           length = len(_x)
           if python3 or type(_x) == unicode:
             _x = _x.encode('utf-8')
             length = len(_x)
           buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-          _x = val2.type
+          _x = val3.type
           buff.write(_get_struct_I().pack(_x))
-          _v2 = val2.pose
-          _v3 = _v2.position
-          _x = _v3
+          _v4 = val3.pose
+          _v5 = _v4.position
+          _x = _v5
           buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-          _v4 = _v2.orientation
-          _x = _v4
+          _v6 = _v4.orientation
+          _x = _v6
           buff.write(_get_struct_4d().pack(_x.x, _x.y, _x.z, _x.w))
-          _x = val2
+          _x = val3
           buff.write(_get_struct_f3IfB().pack(_x.azimuth, _x.image_width, _x.image_height, _x.frame_rate, _x.power, _x.calibrated))
-          _v5 = val2.state
-          _x = _v5
+          _v7 = val3.state
+          _x = _v7
           buff.write(_get_struct_3I().pack(_x.id, _x.state, _x.status))
-          _x = _v5.description
+          _x = _v7.description
           length = len(_x)
           if python3 or type(_x) == unicode:
             _x = _x.encode('utf-8')
             length = len(_x)
           buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-          _x = _v5.lastChange
+          _x = _v7.lastChange
           buff.write(_get_struct_I().pack(_x))
-          length = len(_v5.metrics)
+          length = len(_v7.metrics)
           buff.write(_struct_I.pack(length))
-          for val4 in _v5.metrics:
-            _x = val4.name
+          for val5 in _v7.metrics:
+            _x = val5.name
             length = len(_x)
             if python3 or type(_x) == unicode:
               _x = _x.encode('utf-8')
               length = len(_x)
             buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-            _x = val4.value
+            _x = val5.value
             length = len(_x)
             if python3 or type(_x) == unicode:
               _x = _x.encode('utf-8')
               length = len(_x)
             buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-          _v6 = val2.imu
-          _x = _v6.heading
+          _v8 = val3.imu
+          _x = _v8.heading
           buff.write(_get_struct_f().pack(_x))
-          _x = _v6.device_id
+          _x = _v8.device_id
           length = len(_x)
           if python3 or type(_x) == unicode:
             _x = _x.encode('utf-8')
             length = len(_x)
           buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-          _v7 = _v6.imu
-          _v8 = _v7.header
-          _x = _v8.seq
+          _v9 = _v8.imu
+          _v10 = _v9.header
+          _x = _v10.seq
           buff.write(_get_struct_I().pack(_x))
-          _v9 = _v8.stamp
-          _x = _v9
+          _v11 = _v10.stamp
+          _x = _v11
           buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
-          _x = _v8.frame_id
+          _x = _v10.frame_id
           length = len(_x)
           if python3 or type(_x) == unicode:
             _x = _x.encode('utf-8')
             length = len(_x)
           buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-          _v10 = _v7.orientation
-          _x = _v10
+          _v12 = _v9.orientation
+          _x = _v12
           buff.write(_get_struct_4d().pack(_x.x, _x.y, _x.z, _x.w))
-          buff.write(_get_struct_9d().pack(*_v7.orientation_covariance))
-          _v11 = _v7.angular_velocity
-          _x = _v11
+          buff.write(_get_struct_9d().pack(*_v9.orientation_covariance))
+          _v13 = _v9.angular_velocity
+          _x = _v13
           buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-          buff.write(_get_struct_9d().pack(*_v7.angular_velocity_covariance))
-          _v12 = _v7.linear_acceleration
-          _x = _v12
+          buff.write(_get_struct_9d().pack(*_v9.angular_velocity_covariance))
+          _v14 = _v9.linear_acceleration
+          _x = _v14
           buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-          buff.write(_get_struct_9d().pack(*_v7.linear_acceleration_covariance))
-          _v13 = _v6.magnetic_field
-          _x = _v13
+          buff.write(_get_struct_9d().pack(*_v9.linear_acceleration_covariance))
+          _v15 = _v8.magnetic_field
+          _x = _v15
           buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-          _x = _v6
+          _x = _v8
           buff.write(_get_struct_2fB().pack(_x.roll, _x.pitch, _x.deviceCalibrated))
+        length = len(val1.settings)
+        buff.write(_struct_I.pack(length))
+        for val2 in val1.settings:
+          _x = val2.name
+          length = len(_x)
+          if python3 or type(_x) == unicode:
+            _x = _x.encode('utf-8')
+            length = len(_x)
+          buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+          _x = val2.value
+          length = len(_x)
+          if python3 or type(_x) == unicode:
+            _x = _x.encode('utf-8')
+            length = len(_x)
+          buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
     except struct.error as se: self._check_types(struct.error("%s: '%s' when writing '%s'" % (type(se), str(se), str(locals().get('_x', self)))))
     except TypeError as te: self._check_types(ValueError("%s: '%s' when writing '%s'" % (type(te), str(te), str(locals().get('_x', self)))))
 
   def deserialize(self, str):
     """
     unpack serialized message in str into this message instance
     :param str: byte array of serialized message, ``str``
     """
     if python3:
       codecs.lookup_error("rosmsg").msg_type = self._type
     try:
-      if self.system is None:
-        self.system = digitaleye_msgs.msg.State()
-      if self.components is None:
-        self.components = None
+      if self.position is None:
+        self.position = digitaleye_msgs.msg.Position()
       end = 0
-      _x = self
-      start = end
-      end += 12
-      (_x.system.id, _x.system.state, _x.system.status,) = _get_struct_3I().unpack(str[start:end])
-      start = end
-      end += 4
-      (length,) = _struct_I.unpack(str[start:end])
-      start = end
-      end += length
-      if python3:
-        self.system.description = str[start:end].decode('utf-8', 'rosmsg')
-      else:
-        self.system.description = str[start:end]
-      start = end
-      end += 4
-      (self.system.lastChange,) = _get_struct_I().unpack(str[start:end])
       start = end
       end += 4
       (length,) = _struct_I.unpack(str[start:end])
-      self.system.metrics = []
+      self.position.poles = []
       for i in range(0, length):
-        val1 = digitaleye_msgs.msg.Metric()
+        val1 = digitaleye_msgs.msg.Pole()
+        start = end
+        end += 4
+        (val1.id,) = _get_struct_I().unpack(str[start:end])
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
         start = end
         end += length
         if python3:
-          val1.name = str[start:end].decode('utf-8', 'rosmsg')
+          val1.ip_address = str[start:end].decode('utf-8', 'rosmsg')
         else:
-          val1.name = str[start:end]
+          val1.ip_address = str[start:end]
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
         start = end
         end += length
         if python3:
-          val1.value = str[start:end].decode('utf-8', 'rosmsg')
+          val1.mvc = str[start:end].decode('utf-8', 'rosmsg')
         else:
-          val1.value = str[start:end]
-        self.system.metrics.append(val1)
-      start = end
-      end += 4
-      (length,) = _struct_I.unpack(str[start:end])
-      self.components = []
-      for i in range(0, length):
-        val1 = digitaleye_msgs.msg.ComponentState()
-        _v14 = val1.component
-        _x = _v14
+          val1.mvc = str[start:end]
+        start = end
+        end += 4
+        (length,) = _struct_I.unpack(str[start:end])
+        start = end
+        end += length
+        if python3:
+          val1.iot = str[start:end].decode('utf-8', 'rosmsg')
+        else:
+          val1.iot = str[start:end]
+        start = end
+        end += 4
+        (val1.position_frame,) = _get_struct_I().unpack(str[start:end])
+        _v16 = val1.position
+        _x = _v16
+        start = end
+        end += 24
+        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
+        _x = val1
+        start = end
+        end += 12
+        (_x.orientation_frame, _x.orientation, _x.height,) = _get_struct_I2f().unpack(str[start:end])
+        _v17 = val1.state
+        _v18 = _v17.component
+        _x = _v18
         start = end
         end += 12
         (_x.id, _x.state, _x.status,) = _get_struct_3I().unpack(str[start:end])
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
         start = end
         end += length
         if python3:
-          _v14.description = str[start:end].decode('utf-8', 'rosmsg')
+          _v18.description = str[start:end].decode('utf-8', 'rosmsg')
         else:
-          _v14.description = str[start:end]
+          _v18.description = str[start:end]
         start = end
         end += 4
-        (_v14.lastChange,) = _get_struct_I().unpack(str[start:end])
+        (_v18.lastChange,) = _get_struct_I().unpack(str[start:end])
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
-        _v14.metrics = []
+        _v18.metrics = []
         for i in range(0, length):
-          val3 = digitaleye_msgs.msg.Metric()
+          val4 = digitaleye_msgs.msg.Metric()
           start = end
           end += 4
           (length,) = _struct_I.unpack(str[start:end])
           start = end
           end += length
           if python3:
-            val3.name = str[start:end].decode('utf-8', 'rosmsg')
+            val4.name = str[start:end].decode('utf-8', 'rosmsg')
           else:
-            val3.name = str[start:end]
+            val4.name = str[start:end]
           start = end
           end += 4
           (length,) = _struct_I.unpack(str[start:end])
           start = end
           end += length
           if python3:
-            val3.value = str[start:end].decode('utf-8', 'rosmsg')
+            val4.value = str[start:end].decode('utf-8', 'rosmsg')
           else:
-            val3.value = str[start:end]
-          _v14.metrics.append(val3)
+            val4.value = str[start:end]
+          _v18.metrics.append(val4)
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
-        val1.sensors = []
+        _v17.sensors = []
         for i in range(0, length):
-          val2 = digitaleye_msgs.msg.Sensor()
+          val3 = digitaleye_msgs.msg.Sensor()
           start = end
           end += 4
           (length,) = _struct_I.unpack(str[start:end])
           start = end
           end += length
           if python3:
-            val2.sensor_id = str[start:end].decode('utf-8', 'rosmsg')
+            val3.sensor_id = str[start:end].decode('utf-8', 'rosmsg')
           else:
-            val2.sensor_id = str[start:end]
+            val3.sensor_id = str[start:end]
           start = end
           end += 4
           (length,) = _struct_I.unpack(str[start:end])
           start = end
           end += length
           if python3:
-            val2.model = str[start:end].decode('utf-8', 'rosmsg')
+            val3.model = str[start:end].decode('utf-8', 'rosmsg')
           else:
-            val2.model = str[start:end]
+            val3.model = str[start:end]
           start = end
           end += 4
-          (val2.type,) = _get_struct_I().unpack(str[start:end])
-          _v15 = val2.pose
-          _v16 = _v15.position
-          _x = _v16
+          (val3.type,) = _get_struct_I().unpack(str[start:end])
+          _v19 = val3.pose
+          _v20 = _v19.position
+          _x = _v20
           start = end
           end += 24
           (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-          _v17 = _v15.orientation
-          _x = _v17
+          _v21 = _v19.orientation
+          _x = _v21
           start = end
           end += 32
           (_x.x, _x.y, _x.z, _x.w,) = _get_struct_4d().unpack(str[start:end])
-          _x = val2
+          _x = val3
           start = end
           end += 21
           (_x.azimuth, _x.image_width, _x.image_height, _x.frame_rate, _x.power, _x.calibrated,) = _get_struct_f3IfB().unpack(str[start:end])
-          val2.calibrated = bool(val2.calibrated)
-          _v18 = val2.state
-          _x = _v18
+          val3.calibrated = bool(val3.calibrated)
+          _v22 = val3.state
+          _x = _v22
           start = end
           end += 12
           (_x.id, _x.state, _x.status,) = _get_struct_3I().unpack(str[start:end])
           start = end
           end += 4
           (length,) = _struct_I.unpack(str[start:end])
           start = end
           end += length
           if python3:
-            _v18.description = str[start:end].decode('utf-8', 'rosmsg')
+            _v22.description = str[start:end].decode('utf-8', 'rosmsg')
           else:
-            _v18.description = str[start:end]
+            _v22.description = str[start:end]
           start = end
           end += 4
-          (_v18.lastChange,) = _get_struct_I().unpack(str[start:end])
+          (_v22.lastChange,) = _get_struct_I().unpack(str[start:end])
           start = end
           end += 4
           (length,) = _struct_I.unpack(str[start:end])
-          _v18.metrics = []
+          _v22.metrics = []
           for i in range(0, length):
-            val4 = digitaleye_msgs.msg.Metric()
+            val5 = digitaleye_msgs.msg.Metric()
             start = end
             end += 4
             (length,) = _struct_I.unpack(str[start:end])
             start = end
             end += length
             if python3:
-              val4.name = str[start:end].decode('utf-8', 'rosmsg')
+              val5.name = str[start:end].decode('utf-8', 'rosmsg')
             else:
-              val4.name = str[start:end]
+              val5.name = str[start:end]
             start = end
             end += 4
             (length,) = _struct_I.unpack(str[start:end])
             start = end
             end += length
             if python3:
-              val4.value = str[start:end].decode('utf-8', 'rosmsg')
+              val5.value = str[start:end].decode('utf-8', 'rosmsg')
             else:
-              val4.value = str[start:end]
-            _v18.metrics.append(val4)
-          _v19 = val2.imu
+              val5.value = str[start:end]
+            _v22.metrics.append(val5)
+          _v23 = val3.imu
           start = end
           end += 4
-          (_v19.heading,) = _get_struct_f().unpack(str[start:end])
+          (_v23.heading,) = _get_struct_f().unpack(str[start:end])
           start = end
           end += 4
           (length,) = _struct_I.unpack(str[start:end])
           start = end
           end += length
           if python3:
-            _v19.device_id = str[start:end].decode('utf-8', 'rosmsg')
+            _v23.device_id = str[start:end].decode('utf-8', 'rosmsg')
           else:
-            _v19.device_id = str[start:end]
-          _v20 = _v19.imu
-          _v21 = _v20.header
+            _v23.device_id = str[start:end]
+          _v24 = _v23.imu
+          _v25 = _v24.header
           start = end
           end += 4
-          (_v21.seq,) = _get_struct_I().unpack(str[start:end])
-          _v22 = _v21.stamp
-          _x = _v22
+          (_v25.seq,) = _get_struct_I().unpack(str[start:end])
+          _v26 = _v25.stamp
+          _x = _v26
           start = end
           end += 8
           (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
           start = end
           end += 4
           (length,) = _struct_I.unpack(str[start:end])
           start = end
           end += length
           if python3:
-            _v21.frame_id = str[start:end].decode('utf-8', 'rosmsg')
+            _v25.frame_id = str[start:end].decode('utf-8', 'rosmsg')
           else:
-            _v21.frame_id = str[start:end]
-          _v23 = _v20.orientation
-          _x = _v23
+            _v25.frame_id = str[start:end]
+          _v27 = _v24.orientation
+          _x = _v27
           start = end
           end += 32
           (_x.x, _x.y, _x.z, _x.w,) = _get_struct_4d().unpack(str[start:end])
           start = end
           end += 72
-          _v20.orientation_covariance = _get_struct_9d().unpack(str[start:end])
-          _v24 = _v20.angular_velocity
-          _x = _v24
+          _v24.orientation_covariance = _get_struct_9d().unpack(str[start:end])
+          _v28 = _v24.angular_velocity
+          _x = _v28
           start = end
           end += 24
           (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
           start = end
           end += 72
-          _v20.angular_velocity_covariance = _get_struct_9d().unpack(str[start:end])
-          _v25 = _v20.linear_acceleration
-          _x = _v25
+          _v24.angular_velocity_covariance = _get_struct_9d().unpack(str[start:end])
+          _v29 = _v24.linear_acceleration
+          _x = _v29
           start = end
           end += 24
           (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
           start = end
           end += 72
-          _v20.linear_acceleration_covariance = _get_struct_9d().unpack(str[start:end])
-          _v26 = _v19.magnetic_field
-          _x = _v26
+          _v24.linear_acceleration_covariance = _get_struct_9d().unpack(str[start:end])
+          _v30 = _v23.magnetic_field
+          _x = _v30
           start = end
           end += 24
           (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-          _x = _v19
+          _x = _v23
           start = end
           end += 9
           (_x.roll, _x.pitch, _x.deviceCalibrated,) = _get_struct_2fB().unpack(str[start:end])
-          _v19.deviceCalibrated = bool(_v19.deviceCalibrated)
-          val1.sensors.append(val2)
-        self.components.append(val1)
+          _v23.deviceCalibrated = bool(_v23.deviceCalibrated)
+          _v17.sensors.append(val3)
+        start = end
+        end += 4
+        (length,) = _struct_I.unpack(str[start:end])
+        val1.settings = []
+        for i in range(0, length):
+          val2 = digitaleye_msgs.msg.Metric()
+          start = end
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          start = end
+          end += length
+          if python3:
+            val2.name = str[start:end].decode('utf-8', 'rosmsg')
+          else:
+            val2.name = str[start:end]
+          start = end
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          start = end
+          end += length
+          if python3:
+            val2.value = str[start:end].decode('utf-8', 'rosmsg')
+          else:
+            val2.value = str[start:end]
+          val1.settings.append(val2)
+        self.position.poles.append(val1)
       return self
     except struct.error as e:
       raise genpy.DeserializationError(e)  # most likely buffer underfill
 
 
   def serialize_numpy(self, buff, numpy):
     """
     serialize message with numpy array types into buffer
     :param buff: buffer, ``StringIO``
     :param numpy: numpy python module
     """
     try:
-      _x = self
-      buff.write(_get_struct_3I().pack(_x.system.id, _x.system.state, _x.system.status))
-      _x = self.system.description
-      length = len(_x)
-      if python3 or type(_x) == unicode:
-        _x = _x.encode('utf-8')
-        length = len(_x)
-      buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-      _x = self.system.lastChange
-      buff.write(_get_struct_I().pack(_x))
-      length = len(self.system.metrics)
+      length = len(self.position.poles)
       buff.write(_struct_I.pack(length))
-      for val1 in self.system.metrics:
-        _x = val1.name
+      for val1 in self.position.poles:
+        _x = val1.id
+        buff.write(_get_struct_I().pack(_x))
+        _x = val1.ip_address
         length = len(_x)
         if python3 or type(_x) == unicode:
           _x = _x.encode('utf-8')
           length = len(_x)
         buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = val1.value
+        _x = val1.mvc
         length = len(_x)
         if python3 or type(_x) == unicode:
           _x = _x.encode('utf-8')
           length = len(_x)
         buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-      length = len(self.components)
-      buff.write(_struct_I.pack(length))
-      for val1 in self.components:
-        _v27 = val1.component
-        _x = _v27
+        _x = val1.iot
+        length = len(_x)
+        if python3 or type(_x) == unicode:
+          _x = _x.encode('utf-8')
+          length = len(_x)
+        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+        _x = val1.position_frame
+        buff.write(_get_struct_I().pack(_x))
+        _v31 = val1.position
+        _x = _v31
+        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
+        _x = val1
+        buff.write(_get_struct_I2f().pack(_x.orientation_frame, _x.orientation, _x.height))
+        _v32 = val1.state
+        _v33 = _v32.component
+        _x = _v33
         buff.write(_get_struct_3I().pack(_x.id, _x.state, _x.status))
-        _x = _v27.description
+        _x = _v33.description
         length = len(_x)
         if python3 or type(_x) == unicode:
           _x = _x.encode('utf-8')
           length = len(_x)
         buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = _v27.lastChange
+        _x = _v33.lastChange
         buff.write(_get_struct_I().pack(_x))
-        length = len(_v27.metrics)
+        length = len(_v33.metrics)
         buff.write(_struct_I.pack(length))
-        for val3 in _v27.metrics:
-          _x = val3.name
+        for val4 in _v33.metrics:
+          _x = val4.name
           length = len(_x)
           if python3 or type(_x) == unicode:
             _x = _x.encode('utf-8')
             length = len(_x)
           buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-          _x = val3.value
+          _x = val4.value
           length = len(_x)
           if python3 or type(_x) == unicode:
             _x = _x.encode('utf-8')
             length = len(_x)
           buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        length = len(val1.sensors)
+        length = len(_v32.sensors)
         buff.write(_struct_I.pack(length))
-        for val2 in val1.sensors:
-          _x = val2.sensor_id
+        for val3 in _v32.sensors:
+          _x = val3.sensor_id
           length = len(_x)
           if python3 or type(_x) == unicode:
             _x = _x.encode('utf-8')
             length = len(_x)
           buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-          _x = val2.model
+          _x = val3.model
           length = len(_x)
           if python3 or type(_x) == unicode:
             _x = _x.encode('utf-8')
             length = len(_x)
           buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-          _x = val2.type
+          _x = val3.type
           buff.write(_get_struct_I().pack(_x))
-          _v28 = val2.pose
-          _v29 = _v28.position
-          _x = _v29
+          _v34 = val3.pose
+          _v35 = _v34.position
+          _x = _v35
           buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-          _v30 = _v28.orientation
-          _x = _v30
+          _v36 = _v34.orientation
+          _x = _v36
           buff.write(_get_struct_4d().pack(_x.x, _x.y, _x.z, _x.w))
-          _x = val2
+          _x = val3
           buff.write(_get_struct_f3IfB().pack(_x.azimuth, _x.image_width, _x.image_height, _x.frame_rate, _x.power, _x.calibrated))
-          _v31 = val2.state
-          _x = _v31
+          _v37 = val3.state
+          _x = _v37
           buff.write(_get_struct_3I().pack(_x.id, _x.state, _x.status))
-          _x = _v31.description
+          _x = _v37.description
           length = len(_x)
           if python3 or type(_x) == unicode:
             _x = _x.encode('utf-8')
             length = len(_x)
           buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-          _x = _v31.lastChange
+          _x = _v37.lastChange
           buff.write(_get_struct_I().pack(_x))
-          length = len(_v31.metrics)
+          length = len(_v37.metrics)
           buff.write(_struct_I.pack(length))
-          for val4 in _v31.metrics:
-            _x = val4.name
+          for val5 in _v37.metrics:
+            _x = val5.name
             length = len(_x)
             if python3 or type(_x) == unicode:
               _x = _x.encode('utf-8')
               length = len(_x)
             buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-            _x = val4.value
+            _x = val5.value
             length = len(_x)
             if python3 or type(_x) == unicode:
               _x = _x.encode('utf-8')
               length = len(_x)
             buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-          _v32 = val2.imu
-          _x = _v32.heading
+          _v38 = val3.imu
+          _x = _v38.heading
           buff.write(_get_struct_f().pack(_x))
-          _x = _v32.device_id
+          _x = _v38.device_id
           length = len(_x)
           if python3 or type(_x) == unicode:
             _x = _x.encode('utf-8')
             length = len(_x)
           buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-          _v33 = _v32.imu
-          _v34 = _v33.header
-          _x = _v34.seq
+          _v39 = _v38.imu
+          _v40 = _v39.header
+          _x = _v40.seq
           buff.write(_get_struct_I().pack(_x))
-          _v35 = _v34.stamp
-          _x = _v35
+          _v41 = _v40.stamp
+          _x = _v41
           buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
-          _x = _v34.frame_id
+          _x = _v40.frame_id
           length = len(_x)
           if python3 or type(_x) == unicode:
             _x = _x.encode('utf-8')
             length = len(_x)
           buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-          _v36 = _v33.orientation
-          _x = _v36
+          _v42 = _v39.orientation
+          _x = _v42
           buff.write(_get_struct_4d().pack(_x.x, _x.y, _x.z, _x.w))
-          buff.write(_v33.orientation_covariance.tostring())
-          _v37 = _v33.angular_velocity
-          _x = _v37
+          buff.write(_v39.orientation_covariance.tostring())
+          _v43 = _v39.angular_velocity
+          _x = _v43
           buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-          buff.write(_v33.angular_velocity_covariance.tostring())
-          _v38 = _v33.linear_acceleration
-          _x = _v38
+          buff.write(_v39.angular_velocity_covariance.tostring())
+          _v44 = _v39.linear_acceleration
+          _x = _v44
           buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-          buff.write(_v33.linear_acceleration_covariance.tostring())
-          _v39 = _v32.magnetic_field
-          _x = _v39
+          buff.write(_v39.linear_acceleration_covariance.tostring())
+          _v45 = _v38.magnetic_field
+          _x = _v45
           buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-          _x = _v32
+          _x = _v38
           buff.write(_get_struct_2fB().pack(_x.roll, _x.pitch, _x.deviceCalibrated))
+        length = len(val1.settings)
+        buff.write(_struct_I.pack(length))
+        for val2 in val1.settings:
+          _x = val2.name
+          length = len(_x)
+          if python3 or type(_x) == unicode:
+            _x = _x.encode('utf-8')
+            length = len(_x)
+          buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
+          _x = val2.value
+          length = len(_x)
+          if python3 or type(_x) == unicode:
+            _x = _x.encode('utf-8')
+            length = len(_x)
+          buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
     except struct.error as se: self._check_types(struct.error("%s: '%s' when writing '%s'" % (type(se), str(se), str(locals().get('_x', self)))))
     except TypeError as te: self._check_types(ValueError("%s: '%s' when writing '%s'" % (type(te), str(te), str(locals().get('_x', self)))))
 
   def deserialize_numpy(self, str, numpy):
     """
     unpack serialized message in str into this message instance using numpy for array types
     :param str: byte array of serialized message, ``str``
     :param numpy: numpy python module
     """
     if python3:
       codecs.lookup_error("rosmsg").msg_type = self._type
     try:
-      if self.system is None:
-        self.system = digitaleye_msgs.msg.State()
-      if self.components is None:
-        self.components = None
+      if self.position is None:
+        self.position = digitaleye_msgs.msg.Position()
       end = 0
-      _x = self
-      start = end
-      end += 12
-      (_x.system.id, _x.system.state, _x.system.status,) = _get_struct_3I().unpack(str[start:end])
-      start = end
-      end += 4
-      (length,) = _struct_I.unpack(str[start:end])
-      start = end
-      end += length
-      if python3:
-        self.system.description = str[start:end].decode('utf-8', 'rosmsg')
-      else:
-        self.system.description = str[start:end]
-      start = end
-      end += 4
-      (self.system.lastChange,) = _get_struct_I().unpack(str[start:end])
       start = end
       end += 4
       (length,) = _struct_I.unpack(str[start:end])
-      self.system.metrics = []
+      self.position.poles = []
       for i in range(0, length):
-        val1 = digitaleye_msgs.msg.Metric()
+        val1 = digitaleye_msgs.msg.Pole()
+        start = end
+        end += 4
+        (val1.id,) = _get_struct_I().unpack(str[start:end])
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
         start = end
         end += length
         if python3:
-          val1.name = str[start:end].decode('utf-8', 'rosmsg')
+          val1.ip_address = str[start:end].decode('utf-8', 'rosmsg')
         else:
-          val1.name = str[start:end]
+          val1.ip_address = str[start:end]
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
         start = end
         end += length
         if python3:
-          val1.value = str[start:end].decode('utf-8', 'rosmsg')
+          val1.mvc = str[start:end].decode('utf-8', 'rosmsg')
         else:
-          val1.value = str[start:end]
-        self.system.metrics.append(val1)
-      start = end
-      end += 4
-      (length,) = _struct_I.unpack(str[start:end])
-      self.components = []
-      for i in range(0, length):
-        val1 = digitaleye_msgs.msg.ComponentState()
-        _v40 = val1.component
-        _x = _v40
+          val1.mvc = str[start:end]
+        start = end
+        end += 4
+        (length,) = _struct_I.unpack(str[start:end])
+        start = end
+        end += length
+        if python3:
+          val1.iot = str[start:end].decode('utf-8', 'rosmsg')
+        else:
+          val1.iot = str[start:end]
+        start = end
+        end += 4
+        (val1.position_frame,) = _get_struct_I().unpack(str[start:end])
+        _v46 = val1.position
+        _x = _v46
+        start = end
+        end += 24
+        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
+        _x = val1
+        start = end
+        end += 12
+        (_x.orientation_frame, _x.orientation, _x.height,) = _get_struct_I2f().unpack(str[start:end])
+        _v47 = val1.state
+        _v48 = _v47.component
+        _x = _v48
         start = end
         end += 12
         (_x.id, _x.state, _x.status,) = _get_struct_3I().unpack(str[start:end])
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
         start = end
         end += length
         if python3:
-          _v40.description = str[start:end].decode('utf-8', 'rosmsg')
+          _v48.description = str[start:end].decode('utf-8', 'rosmsg')
         else:
-          _v40.description = str[start:end]
+          _v48.description = str[start:end]
         start = end
         end += 4
-        (_v40.lastChange,) = _get_struct_I().unpack(str[start:end])
+        (_v48.lastChange,) = _get_struct_I().unpack(str[start:end])
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
-        _v40.metrics = []
+        _v48.metrics = []
         for i in range(0, length):
-          val3 = digitaleye_msgs.msg.Metric()
+          val4 = digitaleye_msgs.msg.Metric()
           start = end
           end += 4
           (length,) = _struct_I.unpack(str[start:end])
           start = end
           end += length
           if python3:
-            val3.name = str[start:end].decode('utf-8', 'rosmsg')
+            val4.name = str[start:end].decode('utf-8', 'rosmsg')
           else:
-            val3.name = str[start:end]
+            val4.name = str[start:end]
           start = end
           end += 4
           (length,) = _struct_I.unpack(str[start:end])
           start = end
           end += length
           if python3:
-            val3.value = str[start:end].decode('utf-8', 'rosmsg')
+            val4.value = str[start:end].decode('utf-8', 'rosmsg')
           else:
-            val3.value = str[start:end]
-          _v40.metrics.append(val3)
+            val4.value = str[start:end]
+          _v48.metrics.append(val4)
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
-        val1.sensors = []
+        _v47.sensors = []
         for i in range(0, length):
-          val2 = digitaleye_msgs.msg.Sensor()
+          val3 = digitaleye_msgs.msg.Sensor()
           start = end
           end += 4
           (length,) = _struct_I.unpack(str[start:end])
           start = end
           end += length
           if python3:
-            val2.sensor_id = str[start:end].decode('utf-8', 'rosmsg')
+            val3.sensor_id = str[start:end].decode('utf-8', 'rosmsg')
           else:
-            val2.sensor_id = str[start:end]
+            val3.sensor_id = str[start:end]
           start = end
           end += 4
           (length,) = _struct_I.unpack(str[start:end])
           start = end
           end += length
           if python3:
-            val2.model = str[start:end].decode('utf-8', 'rosmsg')
+            val3.model = str[start:end].decode('utf-8', 'rosmsg')
           else:
-            val2.model = str[start:end]
+            val3.model = str[start:end]
           start = end
           end += 4
-          (val2.type,) = _get_struct_I().unpack(str[start:end])
-          _v41 = val2.pose
-          _v42 = _v41.position
-          _x = _v42
+          (val3.type,) = _get_struct_I().unpack(str[start:end])
+          _v49 = val3.pose
+          _v50 = _v49.position
+          _x = _v50
           start = end
           end += 24
           (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-          _v43 = _v41.orientation
-          _x = _v43
+          _v51 = _v49.orientation
+          _x = _v51
           start = end
           end += 32
           (_x.x, _x.y, _x.z, _x.w,) = _get_struct_4d().unpack(str[start:end])
-          _x = val2
+          _x = val3
           start = end
           end += 21
           (_x.azimuth, _x.image_width, _x.image_height, _x.frame_rate, _x.power, _x.calibrated,) = _get_struct_f3IfB().unpack(str[start:end])
-          val2.calibrated = bool(val2.calibrated)
-          _v44 = val2.state
-          _x = _v44
+          val3.calibrated = bool(val3.calibrated)
+          _v52 = val3.state
+          _x = _v52
           start = end
           end += 12
           (_x.id, _x.state, _x.status,) = _get_struct_3I().unpack(str[start:end])
           start = end
           end += 4
           (length,) = _struct_I.unpack(str[start:end])
           start = end
           end += length
           if python3:
-            _v44.description = str[start:end].decode('utf-8', 'rosmsg')
+            _v52.description = str[start:end].decode('utf-8', 'rosmsg')
           else:
-            _v44.description = str[start:end]
+            _v52.description = str[start:end]
           start = end
           end += 4
-          (_v44.lastChange,) = _get_struct_I().unpack(str[start:end])
+          (_v52.lastChange,) = _get_struct_I().unpack(str[start:end])
           start = end
           end += 4
           (length,) = _struct_I.unpack(str[start:end])
-          _v44.metrics = []
+          _v52.metrics = []
           for i in range(0, length):
-            val4 = digitaleye_msgs.msg.Metric()
+            val5 = digitaleye_msgs.msg.Metric()
             start = end
             end += 4
             (length,) = _struct_I.unpack(str[start:end])
             start = end
             end += length
             if python3:
-              val4.name = str[start:end].decode('utf-8', 'rosmsg')
+              val5.name = str[start:end].decode('utf-8', 'rosmsg')
             else:
-              val4.name = str[start:end]
+              val5.name = str[start:end]
             start = end
             end += 4
             (length,) = _struct_I.unpack(str[start:end])
             start = end
             end += length
             if python3:
-              val4.value = str[start:end].decode('utf-8', 'rosmsg')
+              val5.value = str[start:end].decode('utf-8', 'rosmsg')
             else:
-              val4.value = str[start:end]
-            _v44.metrics.append(val4)
-          _v45 = val2.imu
+              val5.value = str[start:end]
+            _v52.metrics.append(val5)
+          _v53 = val3.imu
           start = end
           end += 4
-          (_v45.heading,) = _get_struct_f().unpack(str[start:end])
+          (_v53.heading,) = _get_struct_f().unpack(str[start:end])
           start = end
           end += 4
           (length,) = _struct_I.unpack(str[start:end])
           start = end
           end += length
           if python3:
-            _v45.device_id = str[start:end].decode('utf-8', 'rosmsg')
+            _v53.device_id = str[start:end].decode('utf-8', 'rosmsg')
           else:
-            _v45.device_id = str[start:end]
-          _v46 = _v45.imu
-          _v47 = _v46.header
+            _v53.device_id = str[start:end]
+          _v54 = _v53.imu
+          _v55 = _v54.header
           start = end
           end += 4
-          (_v47.seq,) = _get_struct_I().unpack(str[start:end])
-          _v48 = _v47.stamp
-          _x = _v48
+          (_v55.seq,) = _get_struct_I().unpack(str[start:end])
+          _v56 = _v55.stamp
+          _x = _v56
           start = end
           end += 8
           (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
           start = end
           end += 4
           (length,) = _struct_I.unpack(str[start:end])
           start = end
           end += length
           if python3:
-            _v47.frame_id = str[start:end].decode('utf-8', 'rosmsg')
+            _v55.frame_id = str[start:end].decode('utf-8', 'rosmsg')
           else:
-            _v47.frame_id = str[start:end]
-          _v49 = _v46.orientation
-          _x = _v49
+            _v55.frame_id = str[start:end]
+          _v57 = _v54.orientation
+          _x = _v57
           start = end
           end += 32
           (_x.x, _x.y, _x.z, _x.w,) = _get_struct_4d().unpack(str[start:end])
           start = end
           end += 72
-          _v46.orientation_covariance = numpy.frombuffer(str[start:end], dtype=numpy.float64, count=9)
-          _v50 = _v46.angular_velocity
-          _x = _v50
+          _v54.orientation_covariance = numpy.frombuffer(str[start:end], dtype=numpy.float64, count=9)
+          _v58 = _v54.angular_velocity
+          _x = _v58
           start = end
           end += 24
           (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
           start = end
           end += 72
-          _v46.angular_velocity_covariance = numpy.frombuffer(str[start:end], dtype=numpy.float64, count=9)
-          _v51 = _v46.linear_acceleration
-          _x = _v51
+          _v54.angular_velocity_covariance = numpy.frombuffer(str[start:end], dtype=numpy.float64, count=9)
+          _v59 = _v54.linear_acceleration
+          _x = _v59
           start = end
           end += 24
           (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
           start = end
           end += 72
-          _v46.linear_acceleration_covariance = numpy.frombuffer(str[start:end], dtype=numpy.float64, count=9)
-          _v52 = _v45.magnetic_field
-          _x = _v52
+          _v54.linear_acceleration_covariance = numpy.frombuffer(str[start:end], dtype=numpy.float64, count=9)
+          _v60 = _v53.magnetic_field
+          _x = _v60
           start = end
           end += 24
           (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-          _x = _v45
+          _x = _v53
           start = end
           end += 9
           (_x.roll, _x.pitch, _x.deviceCalibrated,) = _get_struct_2fB().unpack(str[start:end])
-          _v45.deviceCalibrated = bool(_v45.deviceCalibrated)
-          val1.sensors.append(val2)
-        self.components.append(val1)
+          _v53.deviceCalibrated = bool(_v53.deviceCalibrated)
+          _v47.sensors.append(val3)
+        start = end
+        end += 4
+        (length,) = _struct_I.unpack(str[start:end])
+        val1.settings = []
+        for i in range(0, length):
+          val2 = digitaleye_msgs.msg.Metric()
+          start = end
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          start = end
+          end += length
+          if python3:
+            val2.name = str[start:end].decode('utf-8', 'rosmsg')
+          else:
+            val2.name = str[start:end]
+          start = end
+          end += 4
+          (length,) = _struct_I.unpack(str[start:end])
+          start = end
+          end += length
+          if python3:
+            val2.value = str[start:end].decode('utf-8', 'rosmsg')
+          else:
+            val2.value = str[start:end]
+          val1.settings.append(val2)
+        self.position.poles.append(val1)
       return self
     except struct.error as e:
       raise genpy.DeserializationError(e)  # most likely buffer underfill
 
 _struct_I = genpy.struct_I
 def _get_struct_I():
     global _struct_I
@@ -1118,19 +1341,30 @@
     return _struct_4d
 _struct_9d = None
 def _get_struct_9d():
     global _struct_9d
     if _struct_9d is None:
         _struct_9d = struct.Struct("<9d")
     return _struct_9d
+_struct_I2f = None
+def _get_struct_I2f():
+    global _struct_I2f
+    if _struct_I2f is None:
+        _struct_I2f = struct.Struct("<I2f")
+    return _struct_I2f
 _struct_f = None
 def _get_struct_f():
     global _struct_f
     if _struct_f is None:
         _struct_f = struct.Struct("<f")
     return _struct_f
 _struct_f3IfB = None
 def _get_struct_f3IfB():
     global _struct_f3IfB
     if _struct_f3IfB is None:
         _struct_f3IfB = struct.Struct("<f3IfB")
     return _struct_f3IfB
+class GetPoles(object):
+  _type          = 'digitaleye_msgs/GetPoles'
+  _md5sum = '7495bec4b83825ae9001a24db3ee7d3f'
+  _request_class  = GetPolesRequest
+  _response_class = GetPolesResponse
```

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_SystemTransition.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_SystemTransition.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_TimeSlot.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_TimeSlot.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_UavExtReport.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_UavExtReport.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_UavExtReportList.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_UavExtReportList.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_UavFlightData.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_UavFlightData.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_UavGeneralMsg.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_UavGeneralMsg.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_UavIntReport.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_UavIntReport.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_UavIntReportList.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_UavIntReportList.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_UavState.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_UavState.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_UavStateList.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_UavStateList.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_VehicleCommand.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_VehicleCommand.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Volume.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Volume.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_Zone.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_Zone.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/_ZoneObjectStatus.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/_ZoneObjectStatus.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/msg/__init__.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/msg/__init__.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_BookingUpdate.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_BookingUpdate.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_GetBookingStatus.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetBookingStatus.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_GetBookings.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetBookings.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_GetEntrypoint.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetEntrypoint.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_GetFlightpath.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetFlightpath.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_GetMGSObjects.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetMGSObjects.py`

 * *Files 21% similar despite different names*

```diff
@@ -99,18 +99,17 @@
 import genpy
 import struct
 
 import digitaleye_msgs.msg
 import genpy
 import geometry_msgs.msg
 import std_msgs.msg
-import visualization_msgs.msg
 
 class GetMGSObjectsResponse(genpy.Message):
-  _md5sum = "9c6fa687fce57b83580c917cd7d2aec7"
+  _md5sum = "1649992719988131f7e27dc636f2920e"
   _type = "digitaleye_msgs/GetMGSObjectsResponse"
   _has_header = False  # flag to mark the presence of a Header object
   _full_text = """# PORTAL MGS Objects
 digitaleye_msgs/ObjectList objects
 
 
 ================================================================================
@@ -170,25 +169,26 @@
 # estimated velocity of the object (m/s)
 geometry_msgs/Vector3 velocity
 
 # estimated acceleration of the object (m/s2)
 geometry_msgs/Accel acceleration
 
 # estimated size of the object (meters)
-float32 size
+geometry_msgs/Point scale
 
 # object’s category
 # e.g. Personnel, Package, Passenger, UAV, etc.
 string classification
 
 # list of zone(s) in which the object is
 ZoneObjectStatus[] zones
 
-# Object visualisation marker
-visualization_msgs/Marker bounding_cylinder
+# object’s name
+# e.g. Minion-01 Minion-02, etc.
+string name
 
 ================================================================================
 MSG: geometry_msgs/Point
 # This contains the position of a point in free space
 float64 x
 float64 y
 float64 z
@@ -224,83 +224,14 @@
 # time the object was first detected in this zone
 # (ros timestamp in epoch time)
 time first_detected
 
 # time the object was last detected in this zone
 # (ros timestamp in epoch time)
 time last_detected
-
-================================================================================
-MSG: visualization_msgs/Marker
-# See http://www.ros.org/wiki/rviz/DisplayTypes/Marker and http://www.ros.org/wiki/rviz/Tutorials/Markers%3A%20Basic%20Shapes for more information on using this message with rviz
-
-uint8 ARROW=0
-uint8 CUBE=1
-uint8 SPHERE=2
-uint8 CYLINDER=3
-uint8 LINE_STRIP=4
-uint8 LINE_LIST=5
-uint8 CUBE_LIST=6
-uint8 SPHERE_LIST=7
-uint8 POINTS=8
-uint8 TEXT_VIEW_FACING=9
-uint8 MESH_RESOURCE=10
-uint8 TRIANGLE_LIST=11
-
-uint8 ADD=0
-uint8 MODIFY=0
-uint8 DELETE=2
-uint8 DELETEALL=3
-
-Header header                        # header for time/frame information
-string ns                            # Namespace to place this object in... used in conjunction with id to create a unique name for the object
-int32 id 		                         # object ID useful in conjunction with the namespace for manipulating and deleting the object later
-int32 type 		                       # Type of object
-int32 action 	                       # 0 add/modify an object, 1 (deprecated), 2 deletes an object, 3 deletes all objects
-geometry_msgs/Pose pose                 # Pose of the object
-geometry_msgs/Vector3 scale             # Scale of the object 1,1,1 means default (usually 1 meter square)
-std_msgs/ColorRGBA color             # Color [0.0-1.0]
-duration lifetime                    # How long the object should last before being automatically deleted.  0 means forever
-bool frame_locked                    # If this marker should be frame-locked, i.e. retransformed into its frame every timestep
-
-#Only used if the type specified has some use for them (eg. POINTS, LINE_STRIP, ...)
-geometry_msgs/Point[] points
-#Only used if the type specified has some use for them (eg. POINTS, LINE_STRIP, ...)
-#number of colors must either be 0 or equal to the number of points
-#NOTE: alpha is not yet used
-std_msgs/ColorRGBA[] colors
-
-# NOTE: only used for text markers
-string text
-
-# NOTE: only used for MESH_RESOURCE markers
-string mesh_resource
-bool mesh_use_embedded_materials
-
-================================================================================
-MSG: geometry_msgs/Pose
-# A representation of pose in free space, composed of position and orientation. 
-Point position
-Quaternion orientation
-
-================================================================================
-MSG: geometry_msgs/Quaternion
-# This represents an orientation in free space in quaternion form.
-
-float64 x
-float64 y
-float64 z
-float64 w
-
-================================================================================
-MSG: std_msgs/ColorRGBA
-float32 r
-float32 g
-float32 b
-float32 a
 """
   __slots__ = ['objects']
   _slot_types = ['digitaleye_msgs/ObjectList']
 
   def __init__(self, *args, **kwds):
     """
     Constructor. Any message fields that are implicitly/explicitly
@@ -376,96 +307,40 @@
         _v5 = val1.acceleration
         _v6 = _v5.linear
         _x = _v6
         buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
         _v7 = _v5.angular
         _x = _v7
         buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        _x = val1.size
-        buff.write(_get_struct_f().pack(_x))
+        _v8 = val1.scale
+        _x = _v8
+        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
         _x = val1.classification
         length = len(_x)
         if python3 or type(_x) == unicode:
           _x = _x.encode('utf-8')
           length = len(_x)
         buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
         length = len(val1.zones)
         buff.write(_struct_I.pack(length))
         for val2 in val1.zones:
           _x = val2
           buff.write(_get_struct_IB().pack(_x.zone_id, _x.allowed))
-          _v8 = val2.first_detected
-          _x = _v8
-          buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
-          _v9 = val2.last_detected
+          _v9 = val2.first_detected
           _x = _v9
           buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
-        _v10 = val1.bounding_cylinder
-        _v11 = _v10.header
-        _x = _v11.seq
-        buff.write(_get_struct_I().pack(_x))
-        _v12 = _v11.stamp
-        _x = _v12
-        buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
-        _x = _v11.frame_id
-        length = len(_x)
-        if python3 or type(_x) == unicode:
-          _x = _x.encode('utf-8')
-          length = len(_x)
-        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = _v10.ns
-        length = len(_x)
-        if python3 or type(_x) == unicode:
-          _x = _x.encode('utf-8')
-          length = len(_x)
-        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = _v10
-        buff.write(_get_struct_3i().pack(_x.id, _x.type, _x.action))
-        _v13 = _v10.pose
-        _v14 = _v13.position
-        _x = _v14
-        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        _v15 = _v13.orientation
-        _x = _v15
-        buff.write(_get_struct_4d().pack(_x.x, _x.y, _x.z, _x.w))
-        _v16 = _v10.scale
-        _x = _v16
-        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        _v17 = _v10.color
-        _x = _v17
-        buff.write(_get_struct_4f().pack(_x.r, _x.g, _x.b, _x.a))
-        _v18 = _v10.lifetime
-        _x = _v18
-        buff.write(_get_struct_2i().pack(_x.secs, _x.nsecs))
-        _x = _v10.frame_locked
-        buff.write(_get_struct_B().pack(_x))
-        length = len(_v10.points)
-        buff.write(_struct_I.pack(length))
-        for val3 in _v10.points:
-          _x = val3
-          buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        length = len(_v10.colors)
-        buff.write(_struct_I.pack(length))
-        for val3 in _v10.colors:
-          _x = val3
-          buff.write(_get_struct_4f().pack(_x.r, _x.g, _x.b, _x.a))
-        _x = _v10.text
-        length = len(_x)
-        if python3 or type(_x) == unicode:
-          _x = _x.encode('utf-8')
-          length = len(_x)
-        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = _v10.mesh_resource
+          _v10 = val2.last_detected
+          _x = _v10
+          buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
+        _x = val1.name
         length = len(_x)
         if python3 or type(_x) == unicode:
           _x = _x.encode('utf-8')
           length = len(_x)
         buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = _v10.mesh_use_embedded_materials
-        buff.write(_get_struct_B().pack(_x))
     except struct.error as se: self._check_types(struct.error("%s: '%s' when writing '%s'" % (type(se), str(se), str(locals().get('_x', self)))))
     except TypeError as te: self._check_types(ValueError("%s: '%s' when writing '%s'" % (type(te), str(te), str(locals().get('_x', self)))))
 
   def deserialize(self, str):
     """
     unpack serialized message in str into this message instance
     :param str: byte array of serialized message, ``str``
@@ -491,73 +366,75 @@
         self.objects.header.frame_id = str[start:end]
       start = end
       end += 4
       (length,) = _struct_I.unpack(str[start:end])
       self.objects.objects = []
       for i in range(0, length):
         val1 = digitaleye_msgs.msg.Object()
-        _v19 = val1.header
+        _v11 = val1.header
         start = end
         end += 4
-        (_v19.seq,) = _get_struct_I().unpack(str[start:end])
-        _v20 = _v19.stamp
-        _x = _v20
+        (_v11.seq,) = _get_struct_I().unpack(str[start:end])
+        _v12 = _v11.stamp
+        _x = _v12
         start = end
         end += 8
         (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
         start = end
         end += length
         if python3:
-          _v19.frame_id = str[start:end].decode('utf-8', 'rosmsg')
+          _v11.frame_id = str[start:end].decode('utf-8', 'rosmsg')
         else:
-          _v19.frame_id = str[start:end]
+          _v11.frame_id = str[start:end]
         start = end
         end += 8
         (val1.object_id,) = _get_struct_Q().unpack(str[start:end])
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
         pattern = '<%sQ'%length
         start = end
         s = struct.Struct(pattern)
         end += s.size
         val1.fused_ids = s.unpack(str[start:end])
-        _v21 = val1.position
-        _x = _v21
+        _v13 = val1.position
+        _x = _v13
         start = end
         end += 24
         (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
         start = end
         end += 36
         val1.pos_covariance = _get_struct_9f().unpack(str[start:end])
         start = end
         end += 4
         (val1.accuracy,) = _get_struct_f().unpack(str[start:end])
-        _v22 = val1.velocity
-        _x = _v22
+        _v14 = val1.velocity
+        _x = _v14
         start = end
         end += 24
         (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        _v23 = val1.acceleration
-        _v24 = _v23.linear
-        _x = _v24
+        _v15 = val1.acceleration
+        _v16 = _v15.linear
+        _x = _v16
         start = end
         end += 24
         (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        _v25 = _v23.angular
-        _x = _v25
+        _v17 = _v15.angular
+        _x = _v17
         start = end
         end += 24
         (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
+        _v18 = val1.scale
+        _x = _v18
         start = end
-        end += 4
-        (val1.size,) = _get_struct_f().unpack(str[start:end])
+        end += 24
+        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
         start = end
         end += length
         if python3:
           val1.classification = str[start:end].decode('utf-8', 'rosmsg')
@@ -570,131 +447,34 @@
         for i in range(0, length):
           val2 = digitaleye_msgs.msg.ZoneObjectStatus()
           _x = val2
           start = end
           end += 5
           (_x.zone_id, _x.allowed,) = _get_struct_IB().unpack(str[start:end])
           val2.allowed = bool(val2.allowed)
-          _v26 = val2.first_detected
-          _x = _v26
+          _v19 = val2.first_detected
+          _x = _v19
           start = end
           end += 8
           (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
-          _v27 = val2.last_detected
-          _x = _v27
+          _v20 = val2.last_detected
+          _x = _v20
           start = end
           end += 8
           (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
           val1.zones.append(val2)
-        _v28 = val1.bounding_cylinder
-        _v29 = _v28.header
-        start = end
-        end += 4
-        (_v29.seq,) = _get_struct_I().unpack(str[start:end])
-        _v30 = _v29.stamp
-        _x = _v30
-        start = end
-        end += 8
-        (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
-        start = end
-        end += 4
-        (length,) = _struct_I.unpack(str[start:end])
-        start = end
-        end += length
-        if python3:
-          _v29.frame_id = str[start:end].decode('utf-8', 'rosmsg')
-        else:
-          _v29.frame_id = str[start:end]
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
         start = end
         end += length
         if python3:
-          _v28.ns = str[start:end].decode('utf-8', 'rosmsg')
+          val1.name = str[start:end].decode('utf-8', 'rosmsg')
         else:
-          _v28.ns = str[start:end]
-        _x = _v28
-        start = end
-        end += 12
-        (_x.id, _x.type, _x.action,) = _get_struct_3i().unpack(str[start:end])
-        _v31 = _v28.pose
-        _v32 = _v31.position
-        _x = _v32
-        start = end
-        end += 24
-        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        _v33 = _v31.orientation
-        _x = _v33
-        start = end
-        end += 32
-        (_x.x, _x.y, _x.z, _x.w,) = _get_struct_4d().unpack(str[start:end])
-        _v34 = _v28.scale
-        _x = _v34
-        start = end
-        end += 24
-        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        _v35 = _v28.color
-        _x = _v35
-        start = end
-        end += 16
-        (_x.r, _x.g, _x.b, _x.a,) = _get_struct_4f().unpack(str[start:end])
-        _v36 = _v28.lifetime
-        _x = _v36
-        start = end
-        end += 8
-        (_x.secs, _x.nsecs,) = _get_struct_2i().unpack(str[start:end])
-        start = end
-        end += 1
-        (_v28.frame_locked,) = _get_struct_B().unpack(str[start:end])
-        _v28.frame_locked = bool(_v28.frame_locked)
-        start = end
-        end += 4
-        (length,) = _struct_I.unpack(str[start:end])
-        _v28.points = []
-        for i in range(0, length):
-          val3 = geometry_msgs.msg.Point()
-          _x = val3
-          start = end
-          end += 24
-          (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-          _v28.points.append(val3)
-        start = end
-        end += 4
-        (length,) = _struct_I.unpack(str[start:end])
-        _v28.colors = []
-        for i in range(0, length):
-          val3 = std_msgs.msg.ColorRGBA()
-          _x = val3
-          start = end
-          end += 16
-          (_x.r, _x.g, _x.b, _x.a,) = _get_struct_4f().unpack(str[start:end])
-          _v28.colors.append(val3)
-        start = end
-        end += 4
-        (length,) = _struct_I.unpack(str[start:end])
-        start = end
-        end += length
-        if python3:
-          _v28.text = str[start:end].decode('utf-8', 'rosmsg')
-        else:
-          _v28.text = str[start:end]
-        start = end
-        end += 4
-        (length,) = _struct_I.unpack(str[start:end])
-        start = end
-        end += length
-        if python3:
-          _v28.mesh_resource = str[start:end].decode('utf-8', 'rosmsg')
-        else:
-          _v28.mesh_resource = str[start:end]
-        start = end
-        end += 1
-        (_v28.mesh_use_embedded_materials,) = _get_struct_B().unpack(str[start:end])
-        _v28.mesh_use_embedded_materials = bool(_v28.mesh_use_embedded_materials)
+          val1.name = str[start:end]
         self.objects.objects.append(val1)
       return self
     except struct.error as e:
       raise genpy.DeserializationError(e)  # most likely buffer underfill
 
 
   def serialize_numpy(self, buff, numpy):
@@ -711,130 +491,74 @@
       if python3 or type(_x) == unicode:
         _x = _x.encode('utf-8')
         length = len(_x)
       buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
       length = len(self.objects.objects)
       buff.write(_struct_I.pack(length))
       for val1 in self.objects.objects:
-        _v37 = val1.header
-        _x = _v37.seq
+        _v21 = val1.header
+        _x = _v21.seq
         buff.write(_get_struct_I().pack(_x))
-        _v38 = _v37.stamp
-        _x = _v38
+        _v22 = _v21.stamp
+        _x = _v22
         buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
-        _x = _v37.frame_id
+        _x = _v21.frame_id
         length = len(_x)
         if python3 or type(_x) == unicode:
           _x = _x.encode('utf-8')
           length = len(_x)
         buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
         _x = val1.object_id
         buff.write(_get_struct_Q().pack(_x))
         length = len(val1.fused_ids)
         buff.write(_struct_I.pack(length))
         pattern = '<%sQ'%length
         buff.write(val1.fused_ids.tostring())
-        _v39 = val1.position
-        _x = _v39
+        _v23 = val1.position
+        _x = _v23
         buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
         buff.write(val1.pos_covariance.tostring())
         _x = val1.accuracy
         buff.write(_get_struct_f().pack(_x))
-        _v40 = val1.velocity
-        _x = _v40
+        _v24 = val1.velocity
+        _x = _v24
         buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        _v41 = val1.acceleration
-        _v42 = _v41.linear
-        _x = _v42
+        _v25 = val1.acceleration
+        _v26 = _v25.linear
+        _x = _v26
         buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        _v43 = _v41.angular
-        _x = _v43
+        _v27 = _v25.angular
+        _x = _v27
+        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
+        _v28 = val1.scale
+        _x = _v28
         buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        _x = val1.size
-        buff.write(_get_struct_f().pack(_x))
         _x = val1.classification
         length = len(_x)
         if python3 or type(_x) == unicode:
           _x = _x.encode('utf-8')
           length = len(_x)
         buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
         length = len(val1.zones)
         buff.write(_struct_I.pack(length))
         for val2 in val1.zones:
           _x = val2
           buff.write(_get_struct_IB().pack(_x.zone_id, _x.allowed))
-          _v44 = val2.first_detected
-          _x = _v44
+          _v29 = val2.first_detected
+          _x = _v29
           buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
-          _v45 = val2.last_detected
-          _x = _v45
+          _v30 = val2.last_detected
+          _x = _v30
           buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
-        _v46 = val1.bounding_cylinder
-        _v47 = _v46.header
-        _x = _v47.seq
-        buff.write(_get_struct_I().pack(_x))
-        _v48 = _v47.stamp
-        _x = _v48
-        buff.write(_get_struct_2I().pack(_x.secs, _x.nsecs))
-        _x = _v47.frame_id
-        length = len(_x)
-        if python3 or type(_x) == unicode:
-          _x = _x.encode('utf-8')
-          length = len(_x)
-        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = _v46.ns
-        length = len(_x)
-        if python3 or type(_x) == unicode:
-          _x = _x.encode('utf-8')
-          length = len(_x)
-        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = _v46
-        buff.write(_get_struct_3i().pack(_x.id, _x.type, _x.action))
-        _v49 = _v46.pose
-        _v50 = _v49.position
-        _x = _v50
-        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        _v51 = _v49.orientation
-        _x = _v51
-        buff.write(_get_struct_4d().pack(_x.x, _x.y, _x.z, _x.w))
-        _v52 = _v46.scale
-        _x = _v52
-        buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        _v53 = _v46.color
-        _x = _v53
-        buff.write(_get_struct_4f().pack(_x.r, _x.g, _x.b, _x.a))
-        _v54 = _v46.lifetime
-        _x = _v54
-        buff.write(_get_struct_2i().pack(_x.secs, _x.nsecs))
-        _x = _v46.frame_locked
-        buff.write(_get_struct_B().pack(_x))
-        length = len(_v46.points)
-        buff.write(_struct_I.pack(length))
-        for val3 in _v46.points:
-          _x = val3
-          buff.write(_get_struct_3d().pack(_x.x, _x.y, _x.z))
-        length = len(_v46.colors)
-        buff.write(_struct_I.pack(length))
-        for val3 in _v46.colors:
-          _x = val3
-          buff.write(_get_struct_4f().pack(_x.r, _x.g, _x.b, _x.a))
-        _x = _v46.text
-        length = len(_x)
-        if python3 or type(_x) == unicode:
-          _x = _x.encode('utf-8')
-          length = len(_x)
-        buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = _v46.mesh_resource
+        _x = val1.name
         length = len(_x)
         if python3 or type(_x) == unicode:
           _x = _x.encode('utf-8')
           length = len(_x)
         buff.write(struct.Struct('<I%ss'%length).pack(length, _x))
-        _x = _v46.mesh_use_embedded_materials
-        buff.write(_get_struct_B().pack(_x))
     except struct.error as se: self._check_types(struct.error("%s: '%s' when writing '%s'" % (type(se), str(se), str(locals().get('_x', self)))))
     except TypeError as te: self._check_types(ValueError("%s: '%s' when writing '%s'" % (type(te), str(te), str(locals().get('_x', self)))))
 
   def deserialize_numpy(self, str, numpy):
     """
     unpack serialized message in str into this message instance using numpy for array types
     :param str: byte array of serialized message, ``str``
@@ -861,73 +585,75 @@
         self.objects.header.frame_id = str[start:end]
       start = end
       end += 4
       (length,) = _struct_I.unpack(str[start:end])
       self.objects.objects = []
       for i in range(0, length):
         val1 = digitaleye_msgs.msg.Object()
-        _v55 = val1.header
+        _v31 = val1.header
         start = end
         end += 4
-        (_v55.seq,) = _get_struct_I().unpack(str[start:end])
-        _v56 = _v55.stamp
-        _x = _v56
+        (_v31.seq,) = _get_struct_I().unpack(str[start:end])
+        _v32 = _v31.stamp
+        _x = _v32
         start = end
         end += 8
         (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
         start = end
         end += length
         if python3:
-          _v55.frame_id = str[start:end].decode('utf-8', 'rosmsg')
+          _v31.frame_id = str[start:end].decode('utf-8', 'rosmsg')
         else:
-          _v55.frame_id = str[start:end]
+          _v31.frame_id = str[start:end]
         start = end
         end += 8
         (val1.object_id,) = _get_struct_Q().unpack(str[start:end])
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
         pattern = '<%sQ'%length
         start = end
         s = struct.Struct(pattern)
         end += s.size
         val1.fused_ids = numpy.frombuffer(str[start:end], dtype=numpy.uint64, count=length)
-        _v57 = val1.position
-        _x = _v57
+        _v33 = val1.position
+        _x = _v33
         start = end
         end += 24
         (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
         start = end
         end += 36
         val1.pos_covariance = numpy.frombuffer(str[start:end], dtype=numpy.float32, count=9)
         start = end
         end += 4
         (val1.accuracy,) = _get_struct_f().unpack(str[start:end])
-        _v58 = val1.velocity
-        _x = _v58
+        _v34 = val1.velocity
+        _x = _v34
         start = end
         end += 24
         (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        _v59 = val1.acceleration
-        _v60 = _v59.linear
-        _x = _v60
+        _v35 = val1.acceleration
+        _v36 = _v35.linear
+        _x = _v36
         start = end
         end += 24
         (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        _v61 = _v59.angular
-        _x = _v61
+        _v37 = _v35.angular
+        _x = _v37
         start = end
         end += 24
         (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
+        _v38 = val1.scale
+        _x = _v38
         start = end
-        end += 4
-        (val1.size,) = _get_struct_f().unpack(str[start:end])
+        end += 24
+        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
         start = end
         end += length
         if python3:
           val1.classification = str[start:end].decode('utf-8', 'rosmsg')
@@ -940,131 +666,34 @@
         for i in range(0, length):
           val2 = digitaleye_msgs.msg.ZoneObjectStatus()
           _x = val2
           start = end
           end += 5
           (_x.zone_id, _x.allowed,) = _get_struct_IB().unpack(str[start:end])
           val2.allowed = bool(val2.allowed)
-          _v62 = val2.first_detected
-          _x = _v62
+          _v39 = val2.first_detected
+          _x = _v39
           start = end
           end += 8
           (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
-          _v63 = val2.last_detected
-          _x = _v63
+          _v40 = val2.last_detected
+          _x = _v40
           start = end
           end += 8
           (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
           val1.zones.append(val2)
-        _v64 = val1.bounding_cylinder
-        _v65 = _v64.header
-        start = end
-        end += 4
-        (_v65.seq,) = _get_struct_I().unpack(str[start:end])
-        _v66 = _v65.stamp
-        _x = _v66
-        start = end
-        end += 8
-        (_x.secs, _x.nsecs,) = _get_struct_2I().unpack(str[start:end])
-        start = end
-        end += 4
-        (length,) = _struct_I.unpack(str[start:end])
-        start = end
-        end += length
-        if python3:
-          _v65.frame_id = str[start:end].decode('utf-8', 'rosmsg')
-        else:
-          _v65.frame_id = str[start:end]
-        start = end
-        end += 4
-        (length,) = _struct_I.unpack(str[start:end])
-        start = end
-        end += length
-        if python3:
-          _v64.ns = str[start:end].decode('utf-8', 'rosmsg')
-        else:
-          _v64.ns = str[start:end]
-        _x = _v64
-        start = end
-        end += 12
-        (_x.id, _x.type, _x.action,) = _get_struct_3i().unpack(str[start:end])
-        _v67 = _v64.pose
-        _v68 = _v67.position
-        _x = _v68
-        start = end
-        end += 24
-        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        _v69 = _v67.orientation
-        _x = _v69
-        start = end
-        end += 32
-        (_x.x, _x.y, _x.z, _x.w,) = _get_struct_4d().unpack(str[start:end])
-        _v70 = _v64.scale
-        _x = _v70
-        start = end
-        end += 24
-        (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-        _v71 = _v64.color
-        _x = _v71
-        start = end
-        end += 16
-        (_x.r, _x.g, _x.b, _x.a,) = _get_struct_4f().unpack(str[start:end])
-        _v72 = _v64.lifetime
-        _x = _v72
-        start = end
-        end += 8
-        (_x.secs, _x.nsecs,) = _get_struct_2i().unpack(str[start:end])
-        start = end
-        end += 1
-        (_v64.frame_locked,) = _get_struct_B().unpack(str[start:end])
-        _v64.frame_locked = bool(_v64.frame_locked)
-        start = end
-        end += 4
-        (length,) = _struct_I.unpack(str[start:end])
-        _v64.points = []
-        for i in range(0, length):
-          val3 = geometry_msgs.msg.Point()
-          _x = val3
-          start = end
-          end += 24
-          (_x.x, _x.y, _x.z,) = _get_struct_3d().unpack(str[start:end])
-          _v64.points.append(val3)
-        start = end
-        end += 4
-        (length,) = _struct_I.unpack(str[start:end])
-        _v64.colors = []
-        for i in range(0, length):
-          val3 = std_msgs.msg.ColorRGBA()
-          _x = val3
-          start = end
-          end += 16
-          (_x.r, _x.g, _x.b, _x.a,) = _get_struct_4f().unpack(str[start:end])
-          _v64.colors.append(val3)
-        start = end
-        end += 4
-        (length,) = _struct_I.unpack(str[start:end])
-        start = end
-        end += length
-        if python3:
-          _v64.text = str[start:end].decode('utf-8', 'rosmsg')
-        else:
-          _v64.text = str[start:end]
         start = end
         end += 4
         (length,) = _struct_I.unpack(str[start:end])
         start = end
         end += length
         if python3:
-          _v64.mesh_resource = str[start:end].decode('utf-8', 'rosmsg')
+          val1.name = str[start:end].decode('utf-8', 'rosmsg')
         else:
-          _v64.mesh_resource = str[start:end]
-        start = end
-        end += 1
-        (_v64.mesh_use_embedded_materials,) = _get_struct_B().unpack(str[start:end])
-        _v64.mesh_use_embedded_materials = bool(_v64.mesh_use_embedded_materials)
+          val1.name = str[start:end]
         self.objects.objects.append(val1)
       return self
     except struct.error as e:
       raise genpy.DeserializationError(e)  # most likely buffer underfill
 
 _struct_I = genpy.struct_I
 def _get_struct_I():
@@ -1072,62 +701,32 @@
     return _struct_I
 _struct_2I = None
 def _get_struct_2I():
     global _struct_2I
     if _struct_2I is None:
         _struct_2I = struct.Struct("<2I")
     return _struct_2I
-_struct_2i = None
-def _get_struct_2i():
-    global _struct_2i
-    if _struct_2i is None:
-        _struct_2i = struct.Struct("<2i")
-    return _struct_2i
 _struct_3I = None
 def _get_struct_3I():
     global _struct_3I
     if _struct_3I is None:
         _struct_3I = struct.Struct("<3I")
     return _struct_3I
 _struct_3d = None
 def _get_struct_3d():
     global _struct_3d
     if _struct_3d is None:
         _struct_3d = struct.Struct("<3d")
     return _struct_3d
-_struct_3i = None
-def _get_struct_3i():
-    global _struct_3i
-    if _struct_3i is None:
-        _struct_3i = struct.Struct("<3i")
-    return _struct_3i
-_struct_4d = None
-def _get_struct_4d():
-    global _struct_4d
-    if _struct_4d is None:
-        _struct_4d = struct.Struct("<4d")
-    return _struct_4d
-_struct_4f = None
-def _get_struct_4f():
-    global _struct_4f
-    if _struct_4f is None:
-        _struct_4f = struct.Struct("<4f")
-    return _struct_4f
 _struct_9f = None
 def _get_struct_9f():
     global _struct_9f
     if _struct_9f is None:
         _struct_9f = struct.Struct("<9f")
     return _struct_9f
-_struct_B = None
-def _get_struct_B():
-    global _struct_B
-    if _struct_B is None:
-        _struct_B = struct.Struct("<B")
-    return _struct_B
 _struct_IB = None
 def _get_struct_IB():
     global _struct_IB
     if _struct_IB is None:
         _struct_IB = struct.Struct("<IB")
     return _struct_IB
 _struct_Q = None
@@ -1140,10 +739,10 @@
 def _get_struct_f():
     global _struct_f
     if _struct_f is None:
         _struct_f = struct.Struct("<f")
     return _struct_f
 class GetMGSObjects(object):
   _type          = 'digitaleye_msgs/GetMGSObjects'
-  _md5sum = '9c6fa687fce57b83580c917cd7d2aec7'
+  _md5sum = '1649992719988131f7e27dc636f2920e'
   _request_class  = GetMGSObjectsRequest
   _response_class = GetMGSObjectsResponse
```

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_GetMGSStatus.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetMGSStatus.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_GetNotifications.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetNotifications.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_GetSchedule.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetSchedule.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_GetUAVExternalReport.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetUAVExternalReport.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_GetUAVInternalReport.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetUAVInternalReport.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_GetUavIdInt.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetUavIdInt.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_GetUavIdString.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_GetUavIdString.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_NewBooking.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_NewBooking.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/srv/_PointConversion.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/srv/_PointConversion.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs/srv/__init__.py` & `digitaleye_msgs-1.0.9/digitaleye_msgs/srv/__init__.py`

 * *Files identical despite different names*

### Comparing `digitaleye_msgs-1.0.8/digitaleye_msgs.egg-info/SOURCES.txt` & `digitaleye_msgs-1.0.9/digitaleye_msgs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

