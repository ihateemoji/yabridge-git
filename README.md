# yabridge XBPS Package

This repository contains files for packaging yabridge for Void Linux using the XBPS package manager. The provided template file builds the development version of yabridge as the latest stable version does not work with wine 11+ packaged by Void. This template file installs both yabridge and yabridgectl.

### Installation

1. Clone this repository:
   ```sh
   git clone https://github.com/ihateemoji/yabridge-git.git
   ```
2. Copy the directory to the `srcpkgs` directory in your Void Packages repository:
   ```sh
   cp -r yabridge-git /path/to/void-packages/srcpkgs/
   ```
3. Build the package:
   ```sh
   ./xbps-src pkg yabridge-git
   ```
4. Install the package:
   ```sh
   sudo xbps-install --repository=hostdir/binpkgs yabridge-git
   ```
