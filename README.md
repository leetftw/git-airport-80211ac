# git-airport-80211ac
This repository contains the following compiled binaries:
- Git (no HTTPS support)
- NetBSD 9.0 rescue binaries
These binaries were built to be compatible with the NetBSD 9.0 firmware on Apple AirPort 802.11ac routers. You can find the binaries under the `bin/` folder.

# Credits

## Git
Git is licensed under the GNU General Public License, version 2. See `license/Git.txt` for more information.

Under the GPLv2 I am required to provide source code for any precompiled binaries I share of Git.
You can find a copy of the source tree I used for the build under the `src` folder.
More easily, you can also refer to commit `6fcee4785280a08e7f271bd015a4dc33753e2886` from the upstream repository:
https://git.kernel.org/pub/scm/git/git.git/

## NetBSD
This product includes software developed by the NetBSD Project and its contributors. See `license/NetBSD.txt` for more information.

# Build info
The rescue folder was built by generating a NetBSD 9 sysroot using NetBSD's `build.sh`, compiled for machine evbarm and architecture earmv4. The toolchain and sysroot generated were then used to compile Git.
No modifications were made to the Git or NetBSD source code.
The build process is documented in the accompanying article [to be uploaded](h).
This documentation is provided for transparency and reproducibility but is not required to use the binaries.

# Disclaimer
This product is provided as-is, without any express or implied warranties.
This distribution is not endorsed by:
- The Git Project or its contributors
- The NetBSD Project or its contributors
- Apple Inc.
