# milestonetimeline - Horizontal Milestone Timeline Package

## Description

The `milestonetimeline` package provides a flexible way to create horizontal milestone 
timelines in LaTeX documents with support for date-based positioning, label 
rotation, and per-milestone customization.

## Author

Bret Watson <bret@ticm.com>

## License

GNU General Public License v3.0 (GPL-3.0)

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <https://www.gnu.org/licenses/>.

## Dependencies

- tikz
- xifthen
- xparse
- kvoptions

## Features

- Date-based positioning (ISO format: YYYY-MM-DD)
- Automatic spacing (when no dates provided)
- Customizable label rotation (0°, 45°, 90°)
- Per-milestone height control
- Highlighted milestones (different color/shape)
- Compact and vertical presets
- Date markers on timeline

## Installation

### Option 1: CTAN (Recommended)

```bash
# Once published on CTAN, install via your TeX distribution
tlmgr install milestonetimeline # TeX Live
# or use MiKTeX Console for MiKTeX

## Usage

```latex
\documentclass{article}
\usepackage{milestonetimeline}

\begin{document}
\begin{timeline}[width=14,startdate=2025-01-01,enddate=2025-12-31]
  \milestone[above]{2025-01-15}{Kickoff}
  \milestone[below]{2025-06-30}{Midpoint}
  \highlightmilestone[above]{2025-12-31}{Complete}
\end{timeline}
\end{document}

## Documentation

Run latex dottimeline.dtx to generate documentation.

## Version

1.0 (2026-02-25)

## Bug Reports

Please report issues at: https://github.com/baradhili/latex-linear-milestone-timeline
```
