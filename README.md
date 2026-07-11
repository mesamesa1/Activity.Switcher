Activities Switcher (KDE Plasma 6)

![Activity Switcher Demo](screenshots/output.gif)

Plasma 6 widget designed to switch between Plasma Activities desktops dynamically. It integrates seamlessly into your Plasma panel or sits directly on your desktop as an elegant navigation hub.

Available on [Opendesktop.com](https://www.opendesktop.org/p/2365249/) as a plasmoid

---

Features

Flexible Layouts & Orientation
  - Toggle between **Stacked (Vertical)** and **Side-by-Side (Horizontal)** flows.
  - Automatically adapts to panel thickness or desktop constraints.
  
Shape & Size Customization
  - Multiple button shapes: **Pill**, **Circle**, or **Rectangle**.
  - Custom button widths, heights, scale ratios, and layout spacing.

Theming & Per-Activity Styling
  - Custom **Color Picker** for each running activity.
  - Option to apply custom colors to unselected buttons with custom opacity sliders.
  - **Invert Selection Sizing**: Option to make unselected buttons expand on hover or selection, or shrink/grow based on active states.

Icon & Name Toggle
  - Choose to show names, icons, or both.
  - Comes with clean default vector bubble number icons (`1` and `2`) for your primary activities.
  - Custom **Icon Picker** (using the standard KDE system icon dialog) to set individual activity icons.

Smooth Easing Animations
  - Fully adjustable resize transition durations (from `0ms` up to `5000ms`) with smooth `OutCubic` easing behavior.

---
![Activity Switcher](screenshots/Screenshot_20260711_083426.png)
---

##  Installation

### CLI Installation (Recommended)
You can install the plasmoid locally using Plasma's package manager `kpackagetool6`:

```bash
# Clone the repository
git clone https://github.com/yourusername/com.jmc.activitydesktopswitcher.git
cd com.jmc.activitydesktopswitcher

# Install the widget
kpackagetool6 -i .
```

### Manual Installation
Simply clone or extract the contents to your local Plasma plasmoids directory:

```bash
mkdir -p ~/.local/share/plasma/plasmoids/
cp -r com.jmc.activitydesktopswitcher ~/.local/share/plasma/plasmoids/
```

Then restart `plasmashell` to load the widget:
```bash
plasmashell --replace &
```

---

Configuration Options

Right-click the widget on your desktop or panel and choose **Configure Activity & Desktop Switcher...**:

| Option | Type | Default | Description |
|---|---|---|---|
| **Display Name** | Checkbox | `False` | Show activity names in buttons. |
| **Display Icon** | Checkbox | `False` | Show icons in buttons. |
| **Color Unselected** | Checkbox | `True` | Apply custom color to unselected buttons. |
| **Unselected Opacity** | Slider | `20%` | Transparency level for unselected buttons. |
| **Invert Sizing** | Checkbox | `False` | Expand unselected buttons instead of the selected one. |
| **Sizing Scale Ratio** | Slider | `130%` | Size multiplier for expanded buttons. |
| **Orientation** | Dropdown | `Side-by-side` | Layout flow (Horizontal vs Vertical). |
| **Button Shape** | Dropdown | `Pill` | Choose between Rectangle, Pill, or Circle shapes. |
| **Button Dimensions** | Spinboxes | `40` x `24` | Pixels dimensions for button bounds. |
| **Resize Animation** | Spinbox | `250ms` | Transition duration for pill scaling. |

---

License

This project is licensed under the GPL-3.0 License. Feel free to fork, customize, and share!
