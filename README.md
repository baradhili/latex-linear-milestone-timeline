# dottimeline - LaTeX Timeline Package

A flexible LaTeX package for creating horizontal milestone timelines with date-based positioning.

## Features

- Date-based positioning (ISO format: YYYY-MM-DD)
- Automatic spacing (when no dates provided)
- Customizable label rotation (0°, 45°, 90°)
- Per-milestone height control
- Highlighted milestones (different color/shape)
- Compact and vertical presets
- Date markers on timeline

## Quick Start

```latex
\documentclass{article}
\usepackage{dottimeline}

\begin{document}
\begin{timeline}[width=14,startdate=2025-01-01,enddate=2025-12-31]
  \milestone[above]{2025-01-15}{Kickoff}
  \milestone[below]{2025-06-30}{Midpoint}
  \highlightmilestone[above]{2025-12-31}{Complete}
\end{timeline}
\end{document}