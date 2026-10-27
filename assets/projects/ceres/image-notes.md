# CERES gallery assets

The portfolio entry covers rectification automation and the embedded controller HMI. Stack wording (CODESYS and Structured Text) follows Artem's explicit description. Desktop HMI work is reserved for a separate entry.

- `rectification-equipment.png`: user-supplied engineering render, copied unchanged.
- `rectification-hmi-en.png`: current Ceres PLC rectification HMI demonstration, rendered at 480 × 320 with short English labels and example readings.
- `continuous-column-hmi-en.png`: current Ceres PLC continuous-column HMI demonstration, rendered at 480 × 320 with short English labels and example readings.
- `programmable-controller-en.png`: anonymized English presentation edit of the manufacturer's product photo, https://owen.ru/uploads/613/pr225_iso2.png , discovered on https://owen.ru/upl_files/export/catalog/product.php?cat=plc&prod=pr225&sub=programmiruemie_rele . Generic illustrative screen, not a CERES screenshot or an assertion of firmware compatibility. Manufacturer and model markings removed at Artem's request.

The two HMI images come from the maintained PR225 screen layout in
[CeresMobile](https://github.com/ilinic/CeresMobile/tree/main/docs/design/pr225/en).
Reproduce them with `node docs/design/pr225/render.cjs --lang=en`; the website
uses the lossless `rk-preview.png` and `nbk-preview.png` outputs. The layout,
value positions, status indicators and equipment renders match the current
controller design. Readings are demonstration values. CC means continuous
column; RC means rectification column. The original Russian controller
backgrounds remain available in the source project.

The device photo was edited with the built-in ImageGen tool and retains
transparency. The equipment render is unchanged. The old white HMI presentation
edits have been replaced by the current dark Ceres PLC design.

## Historical ImageGen prompts (previous HMI images and device photo)

### HMI 1

Edit the attached RK.png screenshot, not a redesign. This is an actual low-resolution industrial programmable relay HMI for a rectification column. Preserve the entire original layout, white background, thin gray border, equipment render, blue pipes, dropdown arrows, all numeric readings and original green/gray/black typography. Translate EVERY Cyrillic label to English with no Russian letters left, keeping simple utilitarian low-resolution screen style. Exact replacements: top left РК -> RC; Вкл -> On (both dropdowns); Насос Продукт -> Product pump; л/ч -> L/h; Насос Обр -> Reflux pump; ПГ РК % -> RC heater %; кПа -> kPa; bottom SEL,OK-Ред -> SEL,OK: Edit; ESC-НБК -> ESC: CC; УдержESC-Настр -> Hold ESC: Setup. Other units must be °C. Keep all values 15,37,76,67,89,76,2.1 exactly as in source. Fit English labels within original spaces without overlaps. No new controls, no fancy design, no extra title or watermark. Output this ONE screen only, same aspect ratio.

### HMI 2

Edit the attached NBK.png screenshot, not a redesign. Actual low-resolution industrial programmable relay HMI for a continuous distillation column. Preserve exact original layout, white background, thin gray border, equipment render, pipe colors, dropdown arrows, numeric readings and green/gray/black text styling. Translate EVERY Cyrillic label to English; no Russian letters left. Exact replacements: НБК -> CC; Вкл -> On (both occurrences); ПГ1% -> Heater 1 %; ПГ2% -> Heater 2 %; Насос Бр% -> Feed pump %; Насос Кнл% -> Drain pump %; Насос Гф л/ч -> Heads pump L/h; Насос СС -> Transfer pump; кПа -> kPa; bottom SEL,OK-Ред -> SEL,OK: Edit; ESC-РК -> ESC: RC; УдержESC-Настр -> Hold ESC: Setup. Other units °C. Keep values 67,65,55,25,33,45,0,0,73,0,0 exactly in their original positions. Fit translated labels without overlaps or changing equipment. Keep utilitarian limited-resolution relay screen look; do not modernize, embellish or add title. Output ONE screen only, same aspect ratio.

### Controller

Edit this real product photograph for an anonymous English portfolio presentation. Preserve the exact physical controller, shape, perspective, materials, enclosure, seven buttons, connectors and ports, and transparent background. Do not invent a new controller or change its hardware. Remove the Cyrillic manufacturer logo and Cyrillic model marking at bottom right of the faceplate, leaving that area plain gray. Translate ALL Russian screen text to English, no Cyrillic letters left: title 'COLD SMOKING' may instead be neutral 'PROCESS MONITORING'; 'ТЕМПЕРАТУРА В КАМЕРЕ' -> 'TEMPERATURE'; 'изделие' -> 'Product'; 'ВЛАЖНОСТЬ' -> 'Humidity'; 'МИН' -> 'min'; 'ост. время' -> 'Remaining'; 'МЕНЮ' -> 'MENU'; 'ПУСК' -> 'START'; 'СТОП' -> 'STOP'. Preserve all numeric readouts, units, graph, time, screen layout and realistic limited-resolution look. Physical button labels SEL, OK, ESC, F1, F2, Ethernet, RS-485 and USB remain unchanged. No new branding, CODESYS logo or other labels. Maintain a genuinely transparent background. Output one isolated controller.

