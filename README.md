# Pharmagy Medical App

> 👨‍💻 Developed by **[Suresh Kumar Meesala](https://github.com/SureshKumarMeesala)** · 🎨 UI design by **Adam Sokolowski** (credits below)

A mobile app built with **React Native (0.88+)**, **Expo SDK 58+** and **Expo Router**, using **JavaScript and JSX (`.js`, `.jsx`)**. Every screen is built from the original Sketch design `pharmagy-app-adam_sokolowski.sketch` by **Adam Sokolowski**: one route per artboard, with the artboard's layout, colours, images and text.

![Pharmagy Medical App screens](./showcase.jpg)

## 📱 Screens (4 design artboards)

Listed in the order of the app's flow. "Taps" is the number of tap targets wired on the screen (buttons, tabs, back arrows, list rows).

| # | Screen (artboard) | Route | Size | Taps |
|---|---|---|---|---|
| 1 | **01** · start screen | `src/app/s-01.jsx` | 375 × 809 | 1 |
| 2 | **02** | `src/app/s-02.jsx` | 375 × 809 | 2 |
| 3 | **03** | `src/app/s-03.jsx` | 375 × 809 | 2 |
| 4 | **04** | `src/app/s-04.jsx` | 375 × 809 | 2 |

Screenshots of every screen are in [`screenshots/`](./screenshots).

## 🧩 How it's built

- `src/screens/*.json`: each design artboard converted to screen data (vector shapes, gradients, image fills, masks, shadows, blurs and rich text, positioned as in the design), plus its tap targets
- `src/sketch/SketchScreen.jsx`: draws a screen at the device's width with `react-native-svg`, native `Text`/`TextInput` and `expo-blur`, and handles navigation between screens
- `src/app/`: Expo Router routes, one per artboard (`index.jsx` opens the start screen)
- `assets/images/`: images used by the design

## 🛠️ Tech Stack

- **Framework**: React Native 0.88+ / Expo SDK 58+
- **Navigation**: Expo Router (file-based routing)
- **Language**: JavaScript & JSX (`.js`, `.jsx`)
- **Rendering**: `react-native-svg`, `expo-blur`
- **Fonts**: Google Fonts via `@expo-google-fonts` (DM Sans), standing in for the design's original fonts where those aren't free

<!-- run-locally:start -->

## ▶️ Run locally

```bash
npm install
npx expo start
```

Then press `i` for the iOS simulator, `a` for Android, or `w` for the web, or scan the QR code with Expo Go.

<!-- run-locally:end -->

<!-- developer:start -->

## 👨‍💻 Developer

This React Native app was developed by **Suresh Kumar Meesala**.

| | |
|---|---|
| Developer | [Suresh Kumar Meesala](https://github.com/SureshKumarMeesala) |
| GitHub | [@SureshKumarMeesala](https://github.com/SureshKumarMeesala) |
| Organization | [FreeAppSource](https://github.com/FreeAppSource) |
| Repository | <https://github.com/FreeAppSource/pharmagy-medical-app> |

<!-- developer:end -->

---

<!-- design-credits:start -->

## 🎨 Design Credits

This app is based on the free **Medical Concept App** design by **Adam Sokolowski**, downloaded from Sketch App Sources. All visual design credit goes to the designer. The screens are reproduced from the original Sketch file; fonts that aren't free are replaced with similar Google Fonts, so some details may differ slightly from the original.

| | |
|---|---|
| Designer | [Adam Sokolowski](https://www.sketchappsources.com/contributor/adamsokolowski) |
| Original design | [Medical Concept App](https://dribbble.com/shots/6592169-FREE-Pharmagy-Medical-App-demo) |
| Downloaded from | [Sketch App Sources](https://www.sketchappsources.com/free-source/4180-medical-app-sketch-freebie-resource.html) |
| Website | <https://www.behance.net/rektwondo> |
| Original file | `pharmagy-app-adam_sokolowski.sketch` |
| License / usage | Not stated on the page. Free download; give credit (Sketch App Sources Terms). Confirm with the designer before commercial use. |

**Attribution:**

> UI design: "Medical Concept App" by Adam Sokolowski (https://dribbble.com/shots/6592169-FREE-Pharmagy-Medical-App-demo), downloaded from Sketch App Sources (https://www.sketchappsources.com/free-source/4180-medical-app-sketch-freebie-resource.html).

The original design source files are not included in this repository; get them from the links above. This app's **code** is released under the [MIT License](./LICENSE); the visual design remains the designer's (see [NOTICE](./NOTICE)).

Photos, brand logos and avatars inside the design may belong to third parties and are not covered by the designer's permission.

<!-- design-credits:end -->
