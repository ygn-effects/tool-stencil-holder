# **YGN Stencil Holder**

Our custom made stencil holder provides a quick and easy way to securely hold a PCB and a stencil for precise solder paste application, with different sizes available to match the YGN Framework PCBs.

## **The Problem & Solution**

In industrial manufacturing, solder paste is applied with automated paste printers—a solution that is fast and precise but prohibitively expensive for hobbyists. The common DIY alternatives involve taping an unframed stencil to a workbench or using a framed stencil with a separate, often cumbersome, jig. These methods are prone to error, as even the slightest movement can lead to misaligned paste and faulty solder joints.
The YGN Stencil Holder solves this by providing an affordable, purpose-built tool designed for our framework.

The 3D-printed base has a pocket that precisely matches the PCB dimensions, locking it in place. The top frame then clamps the stencil, using four mounting holes for perfect, repeatable alignment every time.

## **Features**

* **Cost-Effective:** 3D printable on any hobbyist-grade printer, making it incredibly cheap to produce.
* **Minimal Hardware:** Requires only a few common M2 nuts/bolts and two 44mm×32mm hinges, all easily sourced.
* **Precision Fit:** Each holder is designed for a specific YGN PCB, ensuring zero movement and perfect alignment.
* **Fully Open Source:** Designed in FreeCAD, the source files are available for you to inspect, modify, and adapt.

## **File Structure**

The repository is organized by file type (cad for source designs, stl for printable models) and then by size.

```
├── cad
│   ├── small
│   │   ├── stencil-holder-io-board-small-bottom.FCStd
│   │   ├── stencil-holder-io-board-small-top.FCStd
│   │   ├── stencil-holder-small-bottom.FCStd
│   │   └── stencil-holder-small-top.FCStd
│   ├── medium (coming soon)
│   └── large (coming soon)
└── stl
    ├── small
    │   ├── stencil-holder-io-board-small-bottom.step
    │   ├── stencil-holder-io-board-small-top.step
    │   ├── stencil-holder-small-bottom.step
    │   └── stencil-holder-small-top.step
    ├── medium (coming soon)
    └── large (coming soon)
```

## **How to Use**

### **1\. 3D Printing**

Both the top and bottom parts are designed for easy printing on any standard FDM printer.

* The **top** piece can be printed flat on its largest face without any supports.
* The **bottom** piece may require supports for the hexagonal nut traps and the circular recesses for the rubber feet on its underside, depending on your printer's bridging capabilities.


### **2\. Assembly**

Once printed, assembly is straightforward.
**Required Hardware:**

* 2x 32x44mm hinges
* 6x M3x4mm countersunk screws (for the top piece)
* 6x M3x8mm countersunk screws (for the bottom piece)
* 12x M3 nuts

Simply insert the M3 nuts into the hexagonal traps on both the top and bottom pieces. Then, secure the hinges using the screws as shown below.

> **Note:** The hinges have six holes, but using four screws per hinge is typically more than sufficient for a secure fit.

## **Contribution**

This is an open-source project, and contributions are welcome\! If you have an idea for an improvement, find a bug, or want to add a new holder size, please feel free to open an issue or submit a pull request.

**A Note on FreeCAD Files**

This repository uses [zippey](https://github.com/ygn-effects/script-zippey) to make FreeCAD files more friendly for version control. It automatically unpacks the .FCStd file (which is a .zip archive) before committing, allowing Git to track changes to the internal text-based files.

If you plan to contribute changes to the CAD files, please ensure you have `zippey` installed and configured in the repository to maintain a clean and meaningful commit history.

## **License**

This project is released into the public domain under the [CC0 1.0 Universal](https://www.google.com/search?q=LICENSE) license. You are free to use, modify, and distribute the designs and files without restriction.