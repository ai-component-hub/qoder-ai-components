---
name: 'windows-desktop-e2e'
description: 'E2E testing for Windows native desktop apps (WPF, WinForms, Win32/MFC,'
adopted: 2026-05-16
Qt) using pywinauto and Windows UI Automation.
source: everything-claude-code
tier: 2
version: 1.0.0
---

# windows-desktop-e2e

E2E testing for Windows native desktop apps (WPF, WinForms, Win32/MFC, Qt) using pywinauto and Windows UI Automation.

## When to Use

- Use this skill when working on tasks related to windows desktop e2e
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: windows-desktop-e2e
description: E2E testing for Windows native desktop apps (WPF, WinForms, Win32/MFC, Qt) using pywinauto and Windows UI Automation.
origin: ECC
# Windows Desktop E2E Testing
End-to-end testing for Windows native desktop applications using **pywinauto** backed by Windows UI Automation (UIA). Covers WPF, WinForms, Win32/MFC, and Qt (5.x / 6.x) — with Qt-specific guidance as a dedicated section.
## When to Activate
- Writing or running E2E tests for a Windows native desktop application
- Setting up a desktop GUI test suite from scratch
- Diagnosing flaky or failing desktop automation tests
- Adding testability (AutomationId, accessible names) to an existing app
- Integrating desktop E2E into a CI/CD pipeline (GitHub Actions `windows-latest`)
### When NOT to Use
- Web applications → use `e2e-testing` skill (Playwright)
- Electron / CEF / WebView2 apps → the HTML layer needs browser automation, not UIA
- Mobile apps → use platform-specific tools (UIAutomator, XCUITest)
- Pure unit or integration tests that don't need a running GUI
## Core Concepts
All Windows desktop automation relies on **UI Automation (UIA)**, a Windows-built-in accessibility API. Every supported framework exposes a tree of UIA elements with properties Claude can read and act on:
```
Your test (Python)

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: windows-desktop-e2e
