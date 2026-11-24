# Parth Manaktala

> **Save everything. Do nothing. Put a penguin on the Apple Watch.**

I make iPhone apps with very specific opinions. Saving something should work offline. A break shouldn’t come with homework. And a penguin booped on your phone should react on your wrist.

[📸 App screenshots](https://pmanaktala.com/#apps) · [🛠️ Engineering write-ups](https://pmanaktala.com/#work) · [👋 Say hi](https://pmanaktala.com/#contact)

## 🧭 Pick a rabbit hole

| If you want to… | Start here |
| --- | --- |
| 📥 **Rescue something from your 47 open tabs** | **Dump** saves links, images, and notes from the iOS share sheet. Save now, search later. [Get Dump](https://apps.apple.com/us/app/dump-save-anything/id6782526927) |
| 🫧 **Take a break from optimizing your breaks** | **Void** gives you a short pause or guided breathing. Zero streaks to disappoint. [Get Void](https://apps.apple.com/us/app/void-nothing-to-do/id6763810724) |
| 🐧 **See a mood tracker with a penguin in charge** | **Pip** is a one-tap mood log for iPhone and Apple Watch. [Browse the Swift code](https://github.com/pmanaktala/Pip) |
| 🧪 **Give a Spring Boot endpoint some boundaries** | **Restricted Input** lets you reuse validation rules with annotations like `@RestrictedInput`. [See the Java examples](https://github.com/pmanaktala/restricted-input#current-features) |

## 🔧 Under the hood

<details>
<summary><b>🐧 How does a boop get to your wrist?</b></summary>

Pip sends a timestamped event between devices. Each device calculates the animation pose from the scene and the clock. Start with [the pet animation guide](https://github.com/pmanaktala/Pip/blob/main/Docs/Pets/Bible.md), then follow the event through [`DeviceSync`](https://github.com/pmanaktala/Pip/blob/main/PipCore/Services/DeviceSync.swift) and [`PetDirector`](https://github.com/pmanaktala/Pip/blob/main/PipCore/Pet/PetDirector.swift).

</details>

<details>
<summary><b>✈️ What happens when you share a link in airplane mode?</b></summary>

Dump saves it on the device first. Metadata and iCloud sync can catch up later. The share sheet has done its job before the Wi-Fi has a chance to disappoint you.

</details>

By day I work on databases and internal tools, where “OK” can be the start of a bug report. [Read about the controller that said it started](https://pmanaktala.com/#ack).
