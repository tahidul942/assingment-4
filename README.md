# Cookie Cats Retention Analysis Using Bayesian Modeling

This project analyzes the retention rates of players in the mobile game **Cookie Cats** by comparing two versions of the game where a gate was placed at different levels. The analysis uses Bayesian statistical modeling with PyMC to estimate the impact of this gate placement on 1-day and 7-day retention rates.

---

## Table of Contents

1. [Overview](#overview)
2. [Data](#data)
3. [Dependencies](#dependencies)
4. [Code Explanation](#code-explanation)
5. [Results](#results)
6. [Running the Code](#running-the-code)
7. [Contributors](#contributors)

---

## Overview

The goal of this project is to determine whether moving a gate from **Level 30** to **Level 40** affects player retention. The Bayesian approach allows for estimating the posterior distributions of retention rates and the differences between the two versions.

**Key Questions Addressed:**

1. Does the gate placement affect **1-day retention**?
2. Does the gate placement affect **7-day retention**?

---

## Data

The dataset is sourced from the [Cookie Cats dataset](https://github.com/dustywhite7/Econ8310/raw/master/AssignmentData/cookie_cats.csv). It contains information about players who were exposed to different versions of the game:

- **gate_30**: The gate is placed at Level 30.
- **gate_40**: The gate is placed at Level 40.

### Columns in the Dataset

- `userid`: Unique player ID.
- `version`: The version of the game (`gate_30` or `gate_40`).
- `retention_1`: Whether the player returned within 1 day (1 = Yes, 0 = No).
- `retention_7`: Whether the player returned within 7 days (1 = Yes, 0 = No).

---

## Dependencies

To run the code, the following Python libraries are required:

- `pandas`
- `pymc`
- `matplotlib`
- `numpy`

### Install Dependencies

If you're using Google Colab, you can install the dependencies with:

```bash
!pip install pymc matplotlib pandas numpy
