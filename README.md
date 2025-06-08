# Matrix Islands Counter

A simple and interactive web tool to count the number of islands in a binary matrix. Users can input a matrix of 0s and 1s and choose whether to count islands considering diagonal connections or only orthogonal (up, down, left, right) neighbors.

---

## Table of Contents

- [Overview](#overview)
- [Problem Statement](#problem-statement)
- [Features](#features)
- [How It Works](#how-it-works)
- [Usage](#usage)
- [Input Format](#input-format)
- [Technologies Used](#technologies-used)
- [Author](#author)
- [License](#license)

---

## Overview

This web application allows users to paste or type a matrix made up of 0s and 1s, and then calculates the number of islands (connected groups of 1s) either including or excluding diagonal connections.

---

## Problem Statement

Given a matrix consisting of 0s and 1s, count the number of islands. An island is a group of adjacent 1s connected horizontally, vertically, and optionally diagonally.

---

## Features

- Input a binary matrix directly into a text area.
- Validate the matrix format and contents.
- Count islands **with or without** diagonal connectivity.
- Responsive, user-friendly interface.
- Displays error messages for invalid inputs.

---

## How It Works

1. **Parsing Input:** The input string is split by new lines for rows, then by spaces for individual values.
2. **Validation:** Checks that all rows have the same number of columns and only 0s or 1s are present.
3. **Counting Islands:** Uses Depth-First Search (DFS) to traverse and mark connected land cells (1s).
   - If diagonals are included, 8-directional neighbors are considered.
   - Otherwise, only 4-directional neighbors (up, down, left, right) are considered.
4. **Output:** Displays the total island count.

---

## Usage

1. Paste or type your matrix into the input box.
2. Click the button "Count Islands (with Diagonals)" or "Count Islands (without Diagonals)" depending on your preference.
3. The number of islands will be displayed below the buttons.

---

## Input Format

- The matrix should contain only 0s and 1s.
- Rows are separated by newline characters.
- Values in each row are separated by spaces.
