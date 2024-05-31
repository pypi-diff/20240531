# Comparing `tmp/dtschema-2024.4.tar.gz` & `tmp/dtschema-2024.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtschema-2024.4.tar", last modified: Tue Apr 16 20:30:10 2024, max compression
+gzip compressed data, was "dtschema-2024.5.tar", last modified: Fri May 31 17:55:33 2024, max compression
```

## Comparing `dtschema-2024.4.tar` & `dtschema-2024.5.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.869605 dtschema-2024.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.849605 dtschema-2024.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.853605 dtschema-2024.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-16 20:30:06.000000 dtschema-2024.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-16 20:30:06.000000 dtschema-2024.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-16 20:30:06.000000 dtschema-2024.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-16 20:30:06.000000 dtschema-2024.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-04-16 20:30:10.869605 dtschema-2024.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-04-16 20:30:06.000000 dtschema-2024.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.853605 dtschema-2024.4/dtschema/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1531 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/check_compatible.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2028 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/doc_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)    15470 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/dtb.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1306 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/dtb2py.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5937 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/dtb_validate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1200 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/extract_compatibles.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2613 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/extract_example.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1790 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/extract_props.py
--rw-r--r--   0 runner    (1001) docker     (127)    15561 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/fixups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.857605 dtschema-2024.4/dtschema/meta-schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/boolean.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/cell.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/clocks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/core.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/dma.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/gpios.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/hwlock.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/iio.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/interrupts.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/iommu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/items.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/keywords.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/mailbox.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/nodes.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/nvmem.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/phy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/power-domain.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/pwm.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/reset.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/string-array.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/meta-schemas/vendor-props.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)     1326 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/mk_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.861605 dtschema-2024.4/dtschema/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/aliases.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/bootph.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.861605 dtschema-2024.4/dtschema/schemas/bus/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/bus/qemu,platform.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/cache-controller.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/cache.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8432 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/chosen.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.861605 dtschema-2024.4/dtschema/schemas/clock/
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/clock/clock.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/cpu-map.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/cpu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/cpus.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.861605 dtschema-2024.4/dtschema/schemas/dma/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/dma/dma.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/dt-core.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/gpio/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/gpio/gpio-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/gpio/gpio-hog.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/gpio/gpio.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/graph.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/hwlock/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/hwlock/hwlock-consumer.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/i2c/
--rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/i2c/i2c-controller.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/iio/
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/iio/iio-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/iio/iio.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/interconnects.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/interrupt-controller.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/interrupts.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/iommu/
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/iommu/iommu.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/isa/
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/isa/isa-bridge.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/isa/isa-bus.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/mbox/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/mbox/mbox-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/memory.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/msi-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/numa-distance-map-v1.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/opp/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/opp/opp.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/options/
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/options/u-boot.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/options.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/pci/
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/pci/pci-bus-common.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/pci/pci-bus.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/pci/pci-device.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/pci/pci-host-bridge.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/pci/pci-iommu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/pci/pci-pci-bridge.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/phy/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/phy/phy-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/phy/phy-provider.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/pinctrl/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/pinctrl/pinctrl-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/post-init-providers.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/power-domain/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/power-domain/power-domain-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/property-units.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.865605 dtschema-2024.4/dtschema/schemas/pwm/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/pwm/pwm-consumer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/reg.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.869605 dtschema-2024.4/dtschema/schemas/reserved-memory/
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/reserved-memory/framebuffer.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/reserved-memory/memory-region.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/reserved-memory/reserved-memory.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/reserved-memory/shared-dma-pool.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.869605 dtschema-2024.4/dtschema/schemas/reset/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/reset/reset.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/root-node.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/serial.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/simple-bus.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.869605 dtschema-2024.4/dtschema/schemas/thermal/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/thermal/thermal.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/schemas/types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    18559 2024-04-16 20:30:06.000000 dtschema-2024.4/dtschema/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-16 20:30:10.000000 dtschema-2024.4/dtschema/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.869605 dtschema-2024.4/dtschema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-04-16 20:30:10.000000 dtschema-2024.4/dtschema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-16 20:30:10.000000 dtschema-2024.4/dtschema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:30:10.000000 dtschema-2024.4/dtschema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-16 20:30:10.000000 dtschema-2024.4/dtschema.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-16 20:30:10.000000 dtschema-2024.4/dtschema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 20:30:10.000000 dtschema-2024.4/dtschema.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-04-16 20:30:06.000000 dtschema-2024.4/example-schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-16 20:30:06.000000 dtschema-2024.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 20:30:10.873605 dtschema-2024.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.869605 dtschema-2024.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-16 20:30:06.000000 dtschema-2024.4/test/bootphases.dts
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-16 20:30:06.000000 dtschema-2024.4/test/child-node-fail.dts
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-16 20:30:06.000000 dtschema-2024.4/test/child-node.dts
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-16 20:30:06.000000 dtschema-2024.4/test/conditionals-allof-fail.dts
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-16 20:30:06.000000 dtschema-2024.4/test/conditionals-allof-pass.dts
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-16 20:30:06.000000 dtschema-2024.4/test/conditionals-single-fail.dts
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-16 20:30:06.000000 dtschema-2024.4/test/conditionals-single-pass.dts
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-16 20:30:06.000000 dtschema-2024.4/test/device-fail.dts
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-16 20:30:06.000000 dtschema-2024.4/test/device.dts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.869605 dtschema-2024.4/test/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-16 20:30:06.000000 dtschema-2024.4/test/schemas/bad-example.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-16 20:30:06.000000 dtschema-2024.4/test/schemas/child-node-example.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-16 20:30:06.000000 dtschema-2024.4/test/schemas/conditionals-allof-example.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-16 20:30:06.000000 dtschema-2024.4/test/schemas/conditionals-single-example.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-04-16 20:30:06.000000 dtschema-2024.4/test/schemas/good-example.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-16 20:30:06.000000 dtschema-2024.4/test/simple-bus-fail.dts
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-16 20:30:06.000000 dtschema-2024.4/test/simple-bus-pass.dts
--rwxr-xr-x   0 runner    (1001) docker     (127)     5664 2024-04-16 20:30:06.000000 dtschema-2024.4/test/test-dt-validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:30:10.869605 dtschema-2024.4/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6206 2024-04-16 20:30:06.000000 dtschema-2024.4/tools/dt-prop-populate
--rwxr-xr-x   0 runner    (1001) docker     (127)     2135 2024-04-16 20:30:06.000000 dtschema-2024.4/tools/yaml-format
--rwxr-xr-x   0 runner    (1001) docker     (127)      766 2024-04-16 20:30:06.000000 dtschema-2024.4/tools/yaml2json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.334076 dtschema-2024.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.306075 dtschema-2024.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.310076 dtschema-2024.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-31 17:55:28.000000 dtschema-2024.5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-31 17:55:28.000000 dtschema-2024.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-31 17:55:28.000000 dtschema-2024.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-31 17:55:28.000000 dtschema-2024.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-05-31 17:55:33.334076 dtschema-2024.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-05-31 17:55:28.000000 dtschema-2024.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.314076 dtschema-2024.5/dtschema/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1531 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/check_compatible.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2028 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/doc_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15470 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/dtb.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1306 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/dtb2py.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5937 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/dtb_validate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1200 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/extract_compatibles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2613 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/extract_example.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1790 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/extract_props.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15561 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/fixups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.318076 dtschema-2024.5/dtschema/meta-schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/meta-schemas/base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/meta-schemas/boolean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/meta-schemas/cell.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/meta-schemas/clocks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/meta-schemas/core.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/meta-schemas/dma.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/meta-schemas/gpios.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/meta-schemas/hwlock.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/meta-schemas/iio.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/meta-schemas/interrupts.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/meta-schemas/iommu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/meta-schemas/items.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/meta-schemas/keywords.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/meta-schemas/mailbox.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/meta-schemas/nodes.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/meta-schemas/nvmem.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/meta-schemas/phy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/meta-schemas/power-domain.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/meta-schemas/pwm.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/meta-schemas/reset.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/meta-schemas/string-array.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/meta-schemas/types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/meta-schemas/vendor-props.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1326 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/mk_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.322075 dtschema-2024.5/dtschema/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/aliases.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/bootph.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.322075 dtschema-2024.5/dtschema/schemas/bus/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/bus/qemu,platform.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/cache-controller.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/cache.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8432 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/chosen.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.322075 dtschema-2024.5/dtschema/schemas/clock/
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/clock/clock.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/cpu-map.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/cpu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/cpus.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.322075 dtschema-2024.5/dtschema/schemas/dma/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/dma/dma.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/dt-core.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.322075 dtschema-2024.5/dtschema/schemas/gpio/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/gpio/gpio-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/gpio/gpio-hog.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/gpio/gpio.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/graph.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.326076 dtschema-2024.5/dtschema/schemas/hwlock/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/hwlock/hwlock-consumer.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.326076 dtschema-2024.5/dtschema/schemas/i2c/
+-rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/i2c/i2c-controller.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.326076 dtschema-2024.5/dtschema/schemas/iio/
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/iio/iio-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/iio/iio.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/interconnects.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/interrupt-controller.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/interrupts.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.326076 dtschema-2024.5/dtschema/schemas/iommu/
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/iommu/iommu.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.326076 dtschema-2024.5/dtschema/schemas/isa/
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/isa/isa-bridge.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/isa/isa-bus.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.326076 dtschema-2024.5/dtschema/schemas/mbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/mbox/mbox-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/memory.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/msi-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/numa-distance-map-v1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.326076 dtschema-2024.5/dtschema/schemas/opp/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/opp/opp.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.326076 dtschema-2024.5/dtschema/schemas/options/
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/options/u-boot.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/options.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.326076 dtschema-2024.5/dtschema/schemas/pci/
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/pci/pci-bus-common.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/pci/pci-bus.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/pci/pci-device.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/pci/pci-host-bridge.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/pci/pci-iommu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/pci/pci-pci-bridge.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.326076 dtschema-2024.5/dtschema/schemas/phy/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/phy/phy-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/phy/phy-provider.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.326076 dtschema-2024.5/dtschema/schemas/pinctrl/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/pinctrl/pinctrl-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/post-init-providers.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.326076 dtschema-2024.5/dtschema/schemas/power-domain/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/power-domain/power-domain-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/property-units.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.326076 dtschema-2024.5/dtschema/schemas/pwm/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/pwm/pwm-consumer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/reg.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.330076 dtschema-2024.5/dtschema/schemas/reserved-memory/
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/reserved-memory/framebuffer.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/reserved-memory/memory-region.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/reserved-memory/reserved-memory.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/reserved-memory/shared-dma-pool.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.330076 dtschema-2024.5/dtschema/schemas/reset/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/reset/reset.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/root-node.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/serial.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/simple-bus.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.330076 dtschema-2024.5/dtschema/schemas/thermal/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/thermal/thermal.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/schemas/types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    18583 2024-05-31 17:55:28.000000 dtschema-2024.5/dtschema/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-31 17:55:33.000000 dtschema-2024.5/dtschema/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.330076 dtschema-2024.5/dtschema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7900 2024-05-31 17:55:33.000000 dtschema-2024.5/dtschema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-31 17:55:33.000000 dtschema-2024.5/dtschema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 17:55:33.000000 dtschema-2024.5/dtschema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-31 17:55:33.000000 dtschema-2024.5/dtschema.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-31 17:55:33.000000 dtschema-2024.5/dtschema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 17:55:33.000000 dtschema-2024.5/dtschema.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-05-31 17:55:28.000000 dtschema-2024.5/example-schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-31 17:55:28.000000 dtschema-2024.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 17:55:33.334076 dtschema-2024.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.330076 dtschema-2024.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-31 17:55:28.000000 dtschema-2024.5/test/bootphases.dts
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-31 17:55:28.000000 dtschema-2024.5/test/child-node-fail.dts
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-31 17:55:28.000000 dtschema-2024.5/test/child-node.dts
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-31 17:55:28.000000 dtschema-2024.5/test/conditionals-allof-fail.dts
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-31 17:55:28.000000 dtschema-2024.5/test/conditionals-allof-pass.dts
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-31 17:55:28.000000 dtschema-2024.5/test/conditionals-single-fail.dts
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-31 17:55:28.000000 dtschema-2024.5/test/conditionals-single-pass.dts
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-05-31 17:55:28.000000 dtschema-2024.5/test/device-fail.dts
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-31 17:55:28.000000 dtschema-2024.5/test/device.dts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.330076 dtschema-2024.5/test/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-31 17:55:28.000000 dtschema-2024.5/test/schemas/bad-example.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-05-31 17:55:28.000000 dtschema-2024.5/test/schemas/child-node-example.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-31 17:55:28.000000 dtschema-2024.5/test/schemas/conditionals-allof-example.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-31 17:55:28.000000 dtschema-2024.5/test/schemas/conditionals-single-example.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-05-31 17:55:28.000000 dtschema-2024.5/test/schemas/good-example.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-31 17:55:28.000000 dtschema-2024.5/test/simple-bus-fail.dts
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-31 17:55:28.000000 dtschema-2024.5/test/simple-bus-pass.dts
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5664 2024-05-31 17:55:28.000000 dtschema-2024.5/test/test-dt-validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:55:33.330076 dtschema-2024.5/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6206 2024-05-31 17:55:28.000000 dtschema-2024.5/tools/dt-prop-populate
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2135 2024-05-31 17:55:28.000000 dtschema-2024.5/tools/yaml-format
+-rwxr-xr-x   0 runner    (1001) docker     (127)      766 2024-05-31 17:55:28.000000 dtschema-2024.5/tools/yaml2json
```

### Comparing `dtschema-2024.4/.github/workflows/ci.yml` & `dtschema-2024.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/.github/workflows/publish.yml` & `dtschema-2024.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/LICENSE.txt` & `dtschema-2024.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/PKG-INFO` & `dtschema-2024.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtschema
-Version: 2024.4
+Version: 2024.5
 Summary: DeviceTree validation schema and tools
 Author-email: Rob Herring <robh@kernel.org>
 License: Copyright 2018-2019 Linaro Ltd.
         Copyright 2018-2020 Arm Ltd.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
```

### Comparing `dtschema-2024.4/README.md` & `dtschema-2024.5/README.md`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/__init__.py` & `dtschema-2024.5/dtschema/__init__.py`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/check_compatible.py` & `dtschema-2024.5/dtschema/check_compatible.py`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/doc_validate.py` & `dtschema-2024.5/dtschema/doc_validate.py`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/dtb.py` & `dtschema-2024.5/dtschema/dtb.py`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/dtb2py.py` & `dtschema-2024.5/dtschema/dtb2py.py`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/dtb_validate.py` & `dtschema-2024.5/dtschema/dtb_validate.py`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/extract_compatibles.py` & `dtschema-2024.5/dtschema/extract_compatibles.py`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/extract_example.py` & `dtschema-2024.5/dtschema/extract_example.py`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/extract_props.py` & `dtschema-2024.5/dtschema/extract_props.py`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/fixups.py` & `dtschema-2024.5/dtschema/fixups.py`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/lib.py` & `dtschema-2024.5/dtschema/lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # SPDX-License-Identifier: BSD-2-Clause
 # Copyright 2018 Linaro Ltd.
 # Copyright 2018-2023 Arm Ltd.
 # Python library for Devicetree schema validation
 import os
 import re
-import pprint
+
+from jsonschema.exceptions import best_match
 
 # We use a lot of regex's in schema and exceeding the cache size has noticeable
 # peformance impact.
 re._MAXCACHE = 2048
 
 
 class sized_int(int):
@@ -124,29 +125,27 @@
 
     #print(error.__dict__)
     if verbose:
         msg = str(error)
     elif not error.schema_path:
         msg = error.message
     elif error.context:
-        # An error on a conditional will have context with sub-errors
-        msg = "'" + error.schema_path[-1] + "' conditional failed, one must be fixed:"
-
-        for suberror in sorted(error.context, key=lambda e: e.path):
-            if suberror.context:
-                msg += '\n' + format_error(filename, suberror, prefix=prefix+"\t", nodename=nodename, verbose=verbose)
-            elif suberror.message not in msg:
-                msg += '\n' + prefix + '\t' + suberror.message
-                if hasattr(suberror, 'note') and suberror.note and suberror.note != error.note:
-                    msg += '\n\t\t' + prefix + 'hint: ' + suberror.note
-
-    elif error.schema_path[-1] == 'oneOf':
-        msg = 'More than one condition true in oneOf schema:\n\t' + \
-            '\t'.join(pprint.pformat(error.schema, width=72).splitlines(True))
-
+        if len(error.context) == 1:
+            msg = best_match(error.context).message
+        else:
+            # An error on a conditional will have context with sub-errors
+            msg = "'" + error.schema_path[-1] + "' conditional failed, one must be fixed:"
+
+            for suberror in sorted(error.context, key=lambda e: e.path):
+                if suberror.context:
+                    msg += '\n' + format_error(filename, suberror, prefix=prefix+"\t", nodename=nodename, verbose=verbose)
+                elif suberror.message not in msg:
+                    msg += '\n' + prefix + '\t' + suberror.message
+                    if hasattr(suberror, 'note') and suberror.note and suberror.note != error.note:
+                        msg += '\n\t\t' + prefix + 'hint: ' + suberror.note
     else:
         msg = error.message
 
     if hasattr(error, 'note') and error.note:
         msg += '\n\t' + prefix + 'hint: ' + error.note
 
     if hasattr(error, 'schema_file') and error.schema_file:
```

### Comparing `dtschema-2024.4/dtschema/meta-schemas/base.yaml` & `dtschema-2024.5/dtschema/meta-schemas/base.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/meta-schemas/cell.yaml` & `dtschema-2024.5/dtschema/meta-schemas/cell.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/meta-schemas/clocks.yaml` & `dtschema-2024.5/dtschema/meta-schemas/clocks.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/meta-schemas/core.yaml` & `dtschema-2024.5/dtschema/meta-schemas/core.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/meta-schemas/gpios.yaml` & `dtschema-2024.5/dtschema/meta-schemas/gpios.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/meta-schemas/interrupts.yaml` & `dtschema-2024.5/dtschema/meta-schemas/interrupts.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/meta-schemas/items.yaml` & `dtschema-2024.5/dtschema/meta-schemas/items.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/meta-schemas/keywords.yaml` & `dtschema-2024.5/dtschema/meta-schemas/keywords.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/meta-schemas/nodes.yaml` & `dtschema-2024.5/dtschema/meta-schemas/nodes.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/meta-schemas/string-array.yaml` & `dtschema-2024.5/dtschema/meta-schemas/string-array.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/meta-schemas/types.yaml` & `dtschema-2024.5/dtschema/meta-schemas/types.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/meta-schemas/vendor-props.yaml` & `dtschema-2024.5/dtschema/meta-schemas/vendor-props.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/mk_schema.py` & `dtschema-2024.5/dtschema/mk_schema.py`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schema.py` & `dtschema-2024.5/dtschema/schema.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,67 +1,78 @@
 # SPDX-License-Identifier: BSD-2-Clause
 # Copyright 2018 Linaro Ltd.
 # Copyright 2018-2023 Arm Ltd.
 # Python library for Devicetree schema validation
 import sys
 import os
-import ruamel.yaml
 import re
 import copy
 import jsonschema
 
 import dtschema
 
 from jsonschema.exceptions import RefResolutionError
 
 schema_base_url = "http://devicetree.org/"
 schema_basedir = os.path.dirname(os.path.abspath(__file__))
 
-rtyaml = ruamel.yaml.YAML(typ='rt')
-rtyaml.allow_duplicate_keys = False
-rtyaml.preserve_quotes = True
-
-yaml = ruamel.yaml.YAML(typ='safe')
-yaml.allow_duplicate_keys = False
-
 
 def path_to_obj(tree, path):
     for pc in path:
         tree = tree[pc]
     return tree
 
 
 def get_line_col(tree, path, obj=None):
+    import ruamel.yaml
+
     if isinstance(obj, ruamel.yaml.comments.CommentedBase):
         return obj.lc.line, obj.lc.col
     obj = path_to_obj(tree, path)
     if isinstance(obj, ruamel.yaml.comments.CommentedBase):
         return obj.lc.line, obj.lc.col
     if len(path) < 1:
         return -1, -1
     obj = path_to_obj(tree, list(path)[:-1])
     if isinstance(obj, ruamel.yaml.comments.CommentedBase):
         if path[-1] == '$nodename':
             return -1, -1
         return obj.lc.key(path[-1])
     return -1, -1
 
+def _is_node_schema(schema):
+    return isinstance(schema, dict) and \
+           (('type' in schema and schema['type'] == 'object') or
+            schema.keys() & {'properties', 'patternProperties'})
+
+
+def _schema_allows_no_undefined_props(schema):
+    return not schema.get("additionalProperties", True) or \
+           not schema.get("unevaluatedProperties", True)
 
 class DTSchema(dict):
     DtValidator = jsonschema.validators.extend(
         jsonschema.Draft201909Validator,
         format_checker=jsonschema.FormatChecker(),
         version='DT')
 
     def __init__(self, schema_file, line_numbers=False):
         self.paths = [(schema_base_url, schema_basedir + '/')]
         with open(schema_file, 'r', encoding='utf-8') as f:
+            import ruamel.yaml
+
             if line_numbers:
+                rtyaml = ruamel.yaml.YAML(typ='rt')
+                rtyaml.allow_duplicate_keys = False
+                rtyaml.preserve_quotes = True
+
                 schema = rtyaml.load(f.read())
             else:
+                yaml = ruamel.yaml.YAML(typ='safe')
+                yaml.allow_duplicate_keys = False
                 schema = yaml.load(f.read())
 
         self.filename = os.path.abspath(schema_file)
 
         id = schema['$id'].rstrip('#')
         match = re.search('(.*/schemas/)(.+)$', id)
         self.base_path = os.path.abspath(schema_file)[:-len(match[2])]
@@ -72,14 +83,17 @@
         '''Custom handler for http://devicetree.org references'''
         uri = uri.rstrip('#')
         for p in self.paths:
             filename = uri.replace(p[0], p[1])
             if not os.path.isfile(filename):
                 continue
             with open(filename, 'r', encoding='utf-8') as f:
+                import ruamel.yaml
+                yaml = ruamel.yaml.YAML(typ='safe')
+                yaml.allow_duplicate_keys = False
                 return yaml.load(f.read())
 
         raise RefResolutionError('Error in referenced schema matching $id: ' + uri)
 
     def annotate_error(self, error, schema, path):
         error.note = None
         error.schema_file = None
@@ -139,23 +153,44 @@
                 raise scherr
 
     def fixup(self):
         processed_schema = copy.deepcopy(dict(self))
         dtschema.fixups.fixup_schema(processed_schema)
         return processed_schema
 
-    def _check_schema_refs(self, schema):
-        if isinstance(schema, dict) and '$ref' in schema:
-            self.resolver.resolve(schema['$ref'])
-        elif isinstance(schema, dict):
+    def _check_schema_refs(self, schema, parent=None, is_common=False, has_constraint=False):
+        if not parent:
+            is_common = not _schema_allows_no_undefined_props(schema)
+        if isinstance(schema, dict):
+            if parent in {'if', 'select', 'definitions', '$defs', 'then',
+                          'else', 'dependencies', 'dependentSchemas'}:
+                return
+
+            if _is_node_schema(schema):
+                has_constraint = _schema_allows_no_undefined_props(schema)
+
+            if not is_common and _is_node_schema(schema) and \
+               (schema.keys() & {'properties', 'patternProperties', '$ref'}):
+                ref_has_constraint = False
+                if '$ref' in schema:
+                    url, ref_sch = self.resolver.resolve(schema['$ref'])
+
+                    ref_has_constraint = _schema_allows_no_undefined_props(ref_sch)
+                if not ref_has_constraint and \
+                   not (has_constraint or (schema.keys() & {'additionalProperties', 'unevaluatedProperties'})):
+                    print(f"{self.filename}: {parent}: Missing additionalProperties/unevaluatedProperties constraint\n",
+                          file=sys.stderr)
+
             for k, v in schema.items():
-                self._check_schema_refs(v)
+                self._check_schema_refs(v, parent=k, is_common=is_common,
+                                        has_constraint=has_constraint)
         elif isinstance(schema, (list, tuple)):
             for i in range(len(schema)):
-                self._check_schema_refs(schema[i])
+                self._check_schema_refs(schema[i], parent=parent, is_common=is_common,
+                                        has_constraint=has_constraint)
 
     def check_schema_refs(self):
         id = self['$id'].rstrip('#')
         base1 = re.search('schemas/(.+)$', id)[1]
         base2 = self.filename.replace(self.filename[:-len(base1)], '')
         if not base1 == base2:
             print(f"{self.filename}: $id: Cannot determine base path from $id, relative path/filename doesn't match actual path or filename\n",
```

### Comparing `dtschema-2024.4/dtschema/schemas/aliases.yaml` & `dtschema-2024.5/dtschema/schemas/aliases.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/bootph.yaml` & `dtschema-2024.5/dtschema/schemas/bootph.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/bus/qemu,platform.yaml` & `dtschema-2024.5/dtschema/schemas/bus/qemu,platform.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/cache-controller.yaml` & `dtschema-2024.5/dtschema/schemas/cache-controller.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/cache.yaml` & `dtschema-2024.5/dtschema/schemas/cache.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/chosen.yaml` & `dtschema-2024.5/dtschema/schemas/chosen.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/clock/clock.yaml` & `dtschema-2024.5/dtschema/schemas/clock/clock.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/cpu-map.yaml` & `dtschema-2024.5/dtschema/schemas/cpu-map.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/cpu.yaml` & `dtschema-2024.5/dtschema/schemas/cpu.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/cpus.yaml` & `dtschema-2024.5/dtschema/schemas/cpus.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/dma/dma.yaml` & `dtschema-2024.5/dtschema/schemas/dma/dma.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/dt-core.yaml` & `dtschema-2024.5/dtschema/schemas/dt-core.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/gpio/gpio-consumer.yaml` & `dtschema-2024.5/dtschema/schemas/gpio/gpio-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/gpio/gpio-hog.yaml` & `dtschema-2024.5/dtschema/schemas/gpio/gpio-hog.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/gpio/gpio.yaml` & `dtschema-2024.5/dtschema/schemas/gpio/gpio.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/graph.yaml` & `dtschema-2024.5/dtschema/schemas/graph.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/hwlock/hwlock-consumer.yaml` & `dtschema-2024.5/dtschema/schemas/hwlock/hwlock-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/i2c/i2c-controller.yaml` & `dtschema-2024.5/dtschema/schemas/i2c/i2c-controller.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/iio/iio-consumer.yaml` & `dtschema-2024.5/dtschema/schemas/iio/iio-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/iio/iio.yaml` & `dtschema-2024.5/dtschema/schemas/iio/iio.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/interconnects.yaml` & `dtschema-2024.5/dtschema/schemas/interconnects.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/interrupt-controller.yaml` & `dtschema-2024.5/dtschema/schemas/interrupt-controller.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/interrupts.yaml` & `dtschema-2024.5/dtschema/schemas/interrupts.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/iommu/iommu.yaml` & `dtschema-2024.5/dtschema/schemas/iommu/iommu.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/isa/isa-bridge.yaml` & `dtschema-2024.5/dtschema/schemas/isa/isa-bridge.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/isa/isa-bus.yaml` & `dtschema-2024.5/dtschema/schemas/isa/isa-bus.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/mbox/mbox-consumer.yaml` & `dtschema-2024.5/dtschema/schemas/mbox/mbox-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/memory.yaml` & `dtschema-2024.5/dtschema/schemas/memory.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/msi-consumer.yaml` & `dtschema-2024.5/dtschema/schemas/msi-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/numa-distance-map-v1.yaml` & `dtschema-2024.5/dtschema/schemas/numa-distance-map-v1.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/opp/opp.yaml` & `dtschema-2024.5/dtschema/schemas/opp/opp.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/options/u-boot.yaml` & `dtschema-2024.5/dtschema/schemas/options/u-boot.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/options.yaml` & `dtschema-2024.5/dtschema/schemas/options.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/pci/pci-bus-common.yaml` & `dtschema-2024.5/dtschema/schemas/pci/pci-bus-common.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/pci/pci-bus.yaml` & `dtschema-2024.5/dtschema/schemas/pci/pci-bus.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/pci/pci-device.yaml` & `dtschema-2024.5/dtschema/schemas/pci/pci-device.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/pci/pci-host-bridge.yaml` & `dtschema-2024.5/dtschema/schemas/pci/pci-host-bridge.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/pci/pci-iommu.yaml` & `dtschema-2024.5/dtschema/schemas/pci/pci-iommu.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/pci/pci-pci-bridge.yaml` & `dtschema-2024.5/dtschema/schemas/pci/pci-pci-bridge.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/phy/phy-consumer.yaml` & `dtschema-2024.5/dtschema/schemas/phy/phy-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/phy/phy-provider.yaml` & `dtschema-2024.5/dtschema/schemas/phy/phy-provider.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/pinctrl/pinctrl-consumer.yaml` & `dtschema-2024.5/dtschema/schemas/pinctrl/pinctrl-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/post-init-providers.yaml` & `dtschema-2024.5/dtschema/schemas/post-init-providers.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/power-domain/power-domain-consumer.yaml` & `dtschema-2024.5/dtschema/schemas/power-domain/power-domain-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/property-units.yaml` & `dtschema-2024.5/dtschema/schemas/property-units.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/pwm/pwm-consumer.yaml` & `dtschema-2024.5/dtschema/schemas/pwm/pwm-consumer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/reg.yaml` & `dtschema-2024.5/dtschema/schemas/reg.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/reserved-memory/framebuffer.yaml` & `dtschema-2024.5/dtschema/schemas/reserved-memory/framebuffer.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/reserved-memory/memory-region.yaml` & `dtschema-2024.5/dtschema/schemas/reserved-memory/memory-region.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/reserved-memory/reserved-memory.yaml` & `dtschema-2024.5/dtschema/schemas/reserved-memory/reserved-memory.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/reserved-memory/shared-dma-pool.yaml` & `dtschema-2024.5/dtschema/schemas/reserved-memory/shared-dma-pool.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/reset/reset.yaml` & `dtschema-2024.5/dtschema/schemas/reset/reset.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/root-node.yaml` & `dtschema-2024.5/dtschema/schemas/root-node.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/simple-bus.yaml` & `dtschema-2024.5/dtschema/schemas/simple-bus.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -53,19 +53,26 @@
           - $ref: types.yaml#/definitions/flag
     anyOf:
       - required:
           - reg
       - required:
           - ranges
 
-  "^[^@]+$":
-    # Only additional properties should be properties, not nodes.
-    not:
-      type: object
+additionalProperties:
+  description:
+    Anything else must be a property or have empty 'ranges'. An empty 'ranges'
+    is only appropriate if the child node is another 'simple-bus' or similar.
+  if:
+    type: object
+  then:
+    properties:
+      ranges:
+        type: boolean
 
-additionalProperties: false
+    required:
+      - ranges
 
 required:
   - compatible
   - "#address-cells"
   - "#size-cells"
   - ranges
```

### Comparing `dtschema-2024.4/dtschema/schemas/thermal/thermal.yaml` & `dtschema-2024.5/dtschema/schemas/thermal/thermal.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/schemas/types.yaml` & `dtschema-2024.5/dtschema/schemas/types.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/dtschema/validator.py` & `dtschema-2024.5/dtschema/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import os
 import sys
 import re
 import copy
 import glob
 import json
 import jsonschema
-import ruamel.yaml
 
 from jsonschema.exceptions import RefResolutionError
 
 import dtschema
 from dtschema.lib import _is_string_schema
 from dtschema.lib import _get_array_range
 from dtschema.schema import DTSchema
@@ -343,14 +342,15 @@
             # a processed schema file
             with open(schema_files[0], 'r', encoding='utf-8') as f:
                 try:
                     schema_cache = json.load(f)
                 except json.decoder.JSONDecodeError:
                     try:
                         f.seek(0)
+                        import ruamel.yaml
                         yaml = ruamel.yaml.YAML(typ='safe')
                         schema_cache = yaml.load(f.read())
                     except:
                         print("preprocessed schema file is not valid JSON or YAML\n", file=sys.stderr)
                         raise
 
             # Ensure the cache is a processed schema and not just a single schema file
```

### Comparing `dtschema-2024.4/dtschema.egg-info/PKG-INFO` & `dtschema-2024.5/dtschema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtschema
-Version: 2024.4
+Version: 2024.5
 Summary: DeviceTree validation schema and tools
 Author-email: Rob Herring <robh@kernel.org>
 License: Copyright 2018-2019 Linaro Ltd.
         Copyright 2018-2020 Arm Ltd.
         
         Redistribution and use in source and binary forms, with or without modification,
         are permitted provided that the following conditions are met:
```

### Comparing `dtschema-2024.4/dtschema.egg-info/SOURCES.txt` & `dtschema-2024.5/dtschema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/example-schema.yaml` & `dtschema-2024.5/example-schema.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/pyproject.toml` & `dtschema-2024.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/test/child-node-fail.dts` & `dtschema-2024.5/test/child-node-fail.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/test/child-node.dts` & `dtschema-2024.5/test/child-node.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/test/conditionals-allof-fail.dts` & `dtschema-2024.5/test/conditionals-allof-fail.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/test/conditionals-allof-pass.dts` & `dtschema-2024.5/test/conditionals-allof-pass.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/test/conditionals-single-fail.dts` & `dtschema-2024.5/test/conditionals-single-fail.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/test/device-fail.dts` & `dtschema-2024.5/test/device-fail.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/test/device.dts` & `dtschema-2024.5/test/device.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/test/schemas/bad-example.yaml` & `dtschema-2024.5/test/schemas/bad-example.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/test/schemas/child-node-example.yaml` & `dtschema-2024.5/test/schemas/child-node-example.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/test/schemas/conditionals-allof-example.yaml` & `dtschema-2024.5/test/schemas/conditionals-allof-example.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/test/schemas/conditionals-single-example.yaml` & `dtschema-2024.5/test/schemas/conditionals-single-example.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/test/schemas/good-example.yaml` & `dtschema-2024.5/test/schemas/good-example.yaml`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/test/simple-bus-pass.dts` & `dtschema-2024.5/test/simple-bus-pass.dts`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/test/test-dt-validate.py` & `dtschema-2024.5/test/test-dt-validate.py`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/tools/dt-prop-populate` & `dtschema-2024.5/tools/dt-prop-populate`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/tools/yaml-format` & `dtschema-2024.5/tools/yaml-format`

 * *Files identical despite different names*

### Comparing `dtschema-2024.4/tools/yaml2json` & `dtschema-2024.5/tools/yaml2json`

 * *Files identical despite different names*

