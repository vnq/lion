# Change Log

## 0.17.0

### Minor Changes

- 0ddd38c0: member descriptions for editors and api tables

### Patch Changes

- Updated dependencies [0ddd38c0]
- Updated dependencies [0ddd38c0]
  - @lion/form-core@0.13.0
  - @lion/input@0.14.1

## 0.16.0

### Minor Changes

- 02e4f2cb: add simulator to demos

### Patch Changes

- Updated dependencies [11ec31c6]
- Updated dependencies [15146bf9]
- Updated dependencies [02e4f2cb]
- Updated dependencies [c6fbe920]
  - @lion/form-core@0.12.0
  - @lion/core@0.17.0
  - @lion/input@0.14.0

## 0.15.1

### Patch Changes

- Updated dependencies [f0527583]
  - @lion/input@0.13.1

## 0.15.0

### Minor Changes

- 43e4bb81: Type fixes and enhancements:

  - all protected/private entries added to form-core type definitions, and their dependents were fixed
  - a lot @ts-expect-error and @ts-ignore (all `get slots()` and `get modelValue()` issues are fixed)
  - categorized @ts-expect-error / @ts-ignore into:
    - [external]: when a 3rd party didn't ship types (could also be browser specs)
    - [allow-protected]: when we are allowed to know about protected methods. For instance when code
      resides in the same package
    - [allow-private]: when we need to check a private value inside a test
    - [allow]: miscellaneous allows
    - [editor]: when the editor complains, but the cli/ci doesn't

### Patch Changes

- 97b8592c: Remove lion references in docs for easier extending
- Updated dependencies [38297d07]
- Updated dependencies [3b5ed322]
- Updated dependencies [77a04245]
- Updated dependencies [53167fd2]
- Updated dependencies [181a1d45]
- Updated dependencies [fb1522dd]
- Updated dependencies [75af80be]
- Updated dependencies [0e910e3f]
- Updated dependencies [991f1f54]
- Updated dependencies [cc02ae24]
- Updated dependencies [43e4bb81]
- Updated dependencies [6ae7a5e3]
  - @lion/form-core@0.11.0
  - @lion/core@0.16.0
  - @lion/input@0.13.0

## 0.14.3

### Patch Changes

- Updated dependencies [6ea02988]
  - @lion/form-core@0.10.2
  - @lion/input@0.12.3

## 0.14.2

### Patch Changes

- Updated dependencies [72a6ccc8]
  - @lion/form-core@0.10.1
  - @lion/input@0.12.2

## 0.14.1

### Patch Changes

- Updated dependencies [13f808af]
- Updated dependencies [aa478174]
- Updated dependencies [a809d7b5]
  - @lion/form-core@0.10.0
  - @lion/input@0.12.1

## 0.14.0

### Minor Changes

- f3e54c56: Publish documentation with a format for Rocket
- 5db622e9: BREAKING: Align exports fields. This means no more wildcards, meaning you always import with bare import specifiers, extensionless. Import components where customElements.define side effect is executed by importing from '@lion/package/define'. For multi-component packages this defines all components (e.g. radio-group + radio). If you want to only import a single one, do '@lion/radio-group/define-radio' for example for just lion-radio.

### Patch Changes

- Updated dependencies [f3e54c56]
- Updated dependencies [af90b20e]
- Updated dependencies [5db622e9]
  - @lion/core@0.15.0
  - @lion/form-core@0.9.0
  - @lion/input@0.12.0

## 0.13.5

### Patch Changes

- Updated dependencies [dbacafa5]
  - @lion/form-core@0.8.5
  - @lion/input@0.11.5

## 0.13.4

### Patch Changes

- Updated dependencies [6b91c92d]
- Updated dependencies [701aadce]
  - @lion/form-core@0.8.4
  - @lion/core@0.14.1
  - @lion/input@0.11.4

## 0.13.3

### Patch Changes

- Updated dependencies [b2a1c1ef]
  - @lion/form-core@0.8.3
  - @lion/input@0.11.3

## 0.13.2

### Patch Changes

- Updated dependencies [d0b37e62]
  - @lion/form-core@0.8.2
  - @lion/input@0.11.2

## 0.13.1

### Patch Changes

- Updated dependencies [deb95d13]
  - @lion/form-core@0.8.1
  - @lion/input@0.11.1

## 0.13.0

### Minor Changes

- b2f981db: Add exports field in package.json

  Note that some tools can break with this change as long as they respect the exports field. If that is the case, check that you always access the elements included in the exports field, with the same name which they are exported. Any item not exported is considered private to the package and should not be accessed from the outside.

### Patch Changes

- Updated dependencies [b2f981db]
  - @lion/core@0.14.0
  - @lion/form-core@0.8.0
  - @lion/input@0.11.0

## 0.12.16

### Patch Changes

- Updated dependencies [a7b27502]
  - @lion/form-core@0.7.3
  - @lion/input@0.10.16

## 0.12.15

### Patch Changes

- Updated dependencies [77114753]
- Updated dependencies [f98aab23]
- Updated dependencies [f98aab23]
  - @lion/form-core@0.7.2
  - @lion/input@0.10.15

## 0.12.14

### Patch Changes

- 8fb7e7a1: Fix type issues where base constructors would not have the same return type. This allows us to remove a LOT of @ts-expect-errors/@ts-ignores across lion.
- 9112d243: Fix missing types and update to latest scoped elements to fix constructor type.
- Updated dependencies [8fb7e7a1]
- Updated dependencies [9112d243]
  - @lion/core@0.13.8
  - @lion/form-core@0.7.1
  - @lion/input@0.10.14

## 0.12.13

### Patch Changes

- 5302ec89: Minimise dependencies by removing integration demos to form-integrations and form-core packages.
- 98f1bb7e: Ensure all lit imports are imported from @lion/core. Remove devDependencies in all subpackages and move to root package.json. Add demo dependencies as real dependencies for users that extend our docs/demos.
- Updated dependencies [5302ec89]
- Updated dependencies [98f1bb7e]
- Updated dependencies [a8cf4215]
  - @lion/form-core@0.7.0
  - @lion/input@0.10.13
  - @lion/core@0.13.7

## 0.12.12

### Patch Changes

- Updated dependencies [9fba9007]
  - @lion/core@0.13.6
  - @lion/fieldset@0.15.12
  - @lion/form-core@0.6.14
  - @lion/input@0.10.12

## 0.12.11

### Patch Changes

- Updated dependencies [41edf033]
  - @lion/core@0.13.5
  - @lion/fieldset@0.15.11
  - @lion/form-core@0.6.13
  - @lion/input@0.10.11

## 0.12.10

### Patch Changes

- Updated dependencies [5553e43e]
  - @lion/form-core@0.6.12
  - @lion/fieldset@0.15.10
  - @lion/input@0.10.10

## 0.12.9

### Patch Changes

- aa8ad0e6: - (RadioGroup) fix reset bug when selected value was behind inital value
  - Add ChoiceInputMixin test suite
  - Make use of ChoiceGroupMixin test suite
- Updated dependencies [aa8ad0e6]
- Updated dependencies [4bacc17b]
  - @lion/form-core@0.6.11
  - @lion/fieldset@0.15.9
  - @lion/input@0.10.9

## 0.12.8

### Patch Changes

- Updated dependencies [c5c4d4ba]
  - @lion/form-core@0.6.10
  - @lion/fieldset@0.15.8
  - @lion/input@0.10.8

## 0.12.7

### Patch Changes

- Updated dependencies [cf0967fe]
  - @lion/form-core@0.6.9
  - @lion/fieldset@0.15.7
  - @lion/input@0.10.7

## 0.12.6

### Patch Changes

- Updated dependencies [b222fd78]
  - @lion/form-core@0.6.8
  - @lion/fieldset@0.15.6
  - @lion/input@0.10.6

## 0.12.5

### Patch Changes

- cfbcccb5: Fix type imports to reuse lion where possible, in case Lit updates with new types that may break us.
- Updated dependencies [cfbcccb5]
  - @lion/core@0.13.4
  - @lion/form-core@0.6.7
  - @lion/fieldset@0.15.5
  - @lion/input@0.10.5

## 0.12.4

### Patch Changes

- Updated dependencies [e2e4deec]
  - @lion/core@0.13.3
  - @lion/fieldset@0.15.4
  - @lion/form-core@0.6.6
  - @lion/input@0.10.4

## 0.12.3

### Patch Changes

- Updated dependencies [20ba0ca8]
- Updated dependencies [618f2698]
  - @lion/core@0.13.2
  - @lion/form-core@0.6.5
  - @lion/input@0.10.3
  - @lion/fieldset@0.15.3

## 0.12.2

### Patch Changes

- Updated dependencies [2907649b]
- Updated dependencies [68e3e749]
- Updated dependencies [fd297a28]
- Updated dependencies [9fcb67f0]
- Updated dependencies [247e64a3]
- Updated dependencies [e92b98a4]
  - @lion/form-core@0.6.4
  - @lion/core@0.13.1
  - @lion/fieldset@0.15.2
  - @lion/input@0.10.2

## 0.12.1

### Patch Changes

- Updated dependencies [d5faa459]
- Updated dependencies [0aa4480e]
  - @lion/form-core@0.6.3
  - @lion/fieldset@0.15.1
  - @lion/input@0.10.1

## 0.12.0

### Minor Changes

- 50287fba: Added types for the radio-group package.

### Patch Changes

- Updated dependencies [4b7bea96]
- Updated dependencies [01a798e5]
- Updated dependencies [a31b7217]
- Updated dependencies [85720654]
- Updated dependencies [32202a88]
- Updated dependencies [6f08e929]
- Updated dependencies [b9327627]
- Updated dependencies [02145a06]
- Updated dependencies [32202a88]
  - @lion/form-core@0.6.2
  - @lion/core@0.13.0
  - @lion/fieldset@0.15.0
  - @lion/input@0.10.0

## 0.11.16

### Patch Changes

- Updated dependencies [75107a4b]
- Updated dependencies [60d5d1d3]
  - @lion/core@0.12.0
  - @lion/form-core@0.6.1
  - @lion/fieldset@0.14.9
  - @lion/input@0.9.2

## 0.11.15

### Patch Changes

- Updated dependencies [874ff483]
  - @lion/form-core@0.6.0
  - @lion/core@0.11.0
  - @lion/fieldset@0.14.8
  - @lion/input@0.9.1

## 0.11.14

### Patch Changes

- Updated dependencies [65ecd432]
- Updated dependencies [4dc621a0]
  - @lion/core@0.10.0
  - @lion/form-core@0.5.0
  - @lion/input@0.9.0
  - @lion/fieldset@0.14.7

## 0.11.13

### Patch Changes

- Updated dependencies [c347fce4]
  - @lion/fieldset@0.14.6
  - @lion/form-core@0.4.4
  - @lion/input@0.8.6

## 0.11.12

### Patch Changes

- Updated dependencies [4b3ac525]
  - @lion/core@0.9.1
  - @lion/fieldset@0.14.5
  - @lion/form-core@0.4.3
  - @lion/input@0.8.5

## 0.11.11

### Patch Changes

- dd021e43: Groups need a valid formattedValue representing the value of it's form elements
- Updated dependencies [dd021e43]
- Updated dependencies [07c598fd]
  - @lion/fieldset@0.14.4
  - @lion/form-core@0.4.2
  - @lion/input@0.8.4

## 0.11.10

### Patch Changes

- Updated dependencies [fb236975]
  - @lion/form-core@0.4.1
  - @lion/fieldset@0.14.3
  - @lion/input@0.8.3

## 0.11.9

### Patch Changes

- Updated dependencies [3c61fd29]
- Updated dependencies [9ecab4d5]
  - @lion/form-core@0.4.0
  - @lion/core@0.9.0
  - @lion/fieldset@0.14.2
  - @lion/input@0.8.2

All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

## [0.11.8](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.11.7...@lion/radio-group@0.11.8) (2020-07-28)

**Note:** Version bump only for package @lion/radio-group

## [0.11.7](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.11.6...@lion/radio-group@0.11.7) (2020-07-27)

**Note:** Version bump only for package @lion/radio-group

## [0.11.6](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.11.5...@lion/radio-group@0.11.6) (2020-07-16)

**Note:** Version bump only for package @lion/radio-group

## [0.11.5](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.11.4...@lion/radio-group@0.11.5) (2020-07-13)

**Note:** Version bump only for package @lion/radio-group

## [0.11.4](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.11.3...@lion/radio-group@0.11.4) (2020-07-09)

**Note:** Version bump only for package @lion/radio-group

## [0.11.3](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.11.2...@lion/radio-group@0.11.3) (2020-07-09)

**Note:** Version bump only for package @lion/radio-group

## [0.11.2](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.11.1...@lion/radio-group@0.11.2) (2020-07-09)

**Note:** Version bump only for package @lion/radio-group

## [0.11.1](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.11.0...@lion/radio-group@0.11.1) (2020-07-07)

**Note:** Version bump only for package @lion/radio-group

# [0.11.0](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.10.6...@lion/radio-group@0.11.0) (2020-07-06)

### Features

- **choice-input:** add rendering of help-text ([5cd36ca](https://github.com/ing-bank/lion/commit/5cd36cac20c763d47ee495daede421bb66c4d0ba))

## [0.10.6](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.10.5...@lion/radio-group@0.10.6) (2020-06-18)

**Note:** Version bump only for package @lion/radio-group

## [0.10.5](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.10.4...@lion/radio-group@0.10.5) (2020-06-10)

**Note:** Version bump only for package @lion/radio-group

## [0.10.4](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.10.3...@lion/radio-group@0.10.4) (2020-06-09)

**Note:** Version bump only for package @lion/radio-group

## [0.10.3](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.10.2...@lion/radio-group@0.10.3) (2020-06-08)

**Note:** Version bump only for package @lion/radio-group

## [0.10.2](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.10.1...@lion/radio-group@0.10.2) (2020-06-08)

**Note:** Version bump only for package @lion/radio-group

## [0.10.1](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.10.0...@lion/radio-group@0.10.1) (2020-06-03)

### Bug Fixes

- remove all stories folders from npm ([1e04d06](https://github.com/ing-bank/lion/commit/1e04d06921f9d5e1a446b6d14045154ff83771c3))

# [0.10.0](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.9.3...@lion/radio-group@0.10.0) (2020-05-29)

### Features

- merge field/validate/choice-input/form-group into @lion/form-core ([6170374](https://github.com/ing-bank/lion/commit/6170374ee8c058cb95fff79b4953b0535219e9b4))
- use markdown javascript (mdjs) for documentation ([bcd074d](https://github.com/ing-bank/lion/commit/bcd074d1fbce8754d428538df723ba402603e2c8))

## [0.9.3](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.9.2...@lion/radio-group@0.9.3) (2020-05-27)

**Note:** Version bump only for package @lion/radio-group

## [0.9.2](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.9.1...@lion/radio-group@0.9.2) (2020-05-27)

**Note:** Version bump only for package @lion/radio-group

## [0.9.1](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.9.0...@lion/radio-group@0.9.1) (2020-05-25)

**Note:** Version bump only for package @lion/radio-group

# [0.9.0](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.8.8...@lion/radio-group@0.9.0) (2020-05-18)

### Features

- use singleton manager to support nested npm installations ([e2eb0e0](https://github.com/ing-bank/lion/commit/e2eb0e0077b9efed9382701461753778f63cad48))

## [0.8.8](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.8.7...@lion/radio-group@0.8.8) (2020-04-29)

**Note:** Version bump only for package @lion/radio-group

## [0.8.7](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.8.6...@lion/radio-group@0.8.7) (2020-04-02)

**Note:** Version bump only for package @lion/radio-group

## [0.8.6](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.8.5...@lion/radio-group@0.8.6) (2020-03-25)

**Note:** Version bump only for package @lion/radio-group

## [0.8.5](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.8.4...@lion/radio-group@0.8.5) (2020-03-19)

**Note:** Version bump only for package @lion/radio-group

## [0.8.4](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.8.3...@lion/radio-group@0.8.4) (2020-03-12)

**Note:** Version bump only for package @lion/radio-group

## [0.8.3](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.8.2...@lion/radio-group@0.8.3) (2020-03-05)

**Note:** Version bump only for package @lion/radio-group

## [0.8.2](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.8.1...@lion/radio-group@0.8.2) (2020-03-04)

**Note:** Version bump only for package @lion/radio-group

## [0.8.1](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.8.0...@lion/radio-group@0.8.1) (2020-03-02)

**Note:** Version bump only for package @lion/radio-group

# [0.8.0](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.7.1...@lion/radio-group@0.8.0) (2020-03-01)

### Features

- **validate:** use static validatorName instead of instance name ([#600](https://github.com/ing-bank/lion/issues/600)) ([7c45dd6](https://github.com/ing-bank/lion/commit/7c45dd683984e88e3216fba9fcae1b6dc73835b2))

## [0.7.1](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.7.0...@lion/radio-group@0.7.1) (2020-02-26)

**Note:** Version bump only for package @lion/radio-group

# [0.7.0](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.6.3...@lion/radio-group@0.7.0) (2020-02-20)

### Features

- api normalisation formElements and values ([9b905c4](https://github.com/ing-bank/lion/commit/9b905c492a0c0d2226cc1d75c73e2e70dc97815a))

## [0.6.3](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.6.2...@lion/radio-group@0.6.3) (2020-02-19)

### Bug Fixes

- reduce storybook chunck sizes for more performance ([9fc5606](https://github.com/ing-bank/lion/commit/9fc560605f5dcf6e9abcf8d58079c59f12750046))

## [0.6.2](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.6.1...@lion/radio-group@0.6.2) (2020-02-10)

### Bug Fixes

- **checkbox-group:** throw if name does not contain [](<[5957cd9](https://github.com/ing-bank/lion/commit/5957cd916507c36e424d795e52112c8c623fd29c)>)
- move documentation from readme to mdx ([d2708d2](https://github.com/ing-bank/lion/commit/d2708d2457e4af9685f76f9d0eb3cdf549b16ab7))

## [0.6.1](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.6.0...@lion/radio-group@0.6.1) (2020-02-10)

**Note:** Version bump only for package @lion/radio-group

# [0.6.0](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.5.9...@lion/radio-group@0.6.0) (2020-02-06)

### Features

- flatten modelValue and remove checkedValue ([848ff06](https://github.com/ing-bank/lion/commit/848ff06887c86532e60d33d2db67d1152910d9cb))

## [0.5.9](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.5.8...@lion/radio-group@0.5.9) (2020-02-06)

**Note:** Version bump only for package @lion/radio-group

## [0.5.8](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.5.7...@lion/radio-group@0.5.8) (2020-02-06)

**Note:** Version bump only for package @lion/radio-group

## [0.5.7](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.5.6...@lion/radio-group@0.5.7) (2020-02-05)

**Note:** Version bump only for package @lion/radio-group

## [0.5.6](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.5.5...@lion/radio-group@0.5.6) (2020-02-05)

**Note:** Version bump only for package @lion/radio-group

## [0.5.5](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.5.4...@lion/radio-group@0.5.5) (2020-02-03)

**Note:** Version bump only for package @lion/radio-group

## [0.5.4](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.5.3...@lion/radio-group@0.5.4) (2020-01-23)

### Bug Fixes

- update links in stories ([0c53b1d](https://github.com/ing-bank/lion/commit/0c53b1d4bb4fa51820656bacfc2aece653d03182))

## [0.5.3](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.5.2...@lion/radio-group@0.5.3) (2020-01-23)

**Note:** Version bump only for package @lion/radio-group

## [0.5.2](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.5.1...@lion/radio-group@0.5.2) (2020-01-20)

**Note:** Version bump only for package @lion/radio-group

## [0.5.1](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.5.0...@lion/radio-group@0.5.1) (2020-01-17)

### Bug Fixes

- update storybook and use main.js ([e61e0b9](https://github.com/ing-bank/lion/commit/e61e0b938ff72cc18cc0b3aa1560f2cece0c9fe6))

# [0.5.0](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.4.5...@lion/radio-group@0.5.0) (2020-01-13)

### Features

- improved storybook demos ([89b835a](https://github.com/ing-bank/lion/commit/89b835a79998c45a28093de01f69216c35009a40))

## [0.4.5](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.4.4...@lion/radio-group@0.4.5) (2020-01-08)

**Note:** Version bump only for package @lion/radio-group

## [0.4.4](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.4.3...@lion/radio-group@0.4.4) (2019-12-16)

**Note:** Version bump only for package @lion/radio-group

## [0.4.3](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.4.2...@lion/radio-group@0.4.3) (2019-12-13)

**Note:** Version bump only for package @lion/radio-group

## [0.4.2](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.4.1...@lion/radio-group@0.4.2) (2019-12-11)

### Bug Fixes

- **lion-radio-group:** wait for registration before setting values ([#421](https://github.com/ing-bank/lion/issues/421)) ([4dbd737](https://github.com/ing-bank/lion/commit/4dbd73795f2b10e61d12804eb488a0b6b583245e))

## [0.4.1](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.4.0...@lion/radio-group@0.4.1) (2019-12-11)

**Note:** Version bump only for package @lion/radio-group

# [0.4.0](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.3.8...@lion/radio-group@0.4.0) (2019-12-04)

### Features

- integrate and pass automated a11y testing ([e1a417b](https://github.com/ing-bank/lion/commit/e1a417b041431e4e25a5b6a63e23ba0a3974f5a5))

## [0.3.8](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.3.7...@lion/radio-group@0.3.8) (2019-12-03)

### Bug Fixes

- let lerna publish fixed versions ([bc7448c](https://github.com/ing-bank/lion/commit/bc7448c694deb3c05fd3d083a9acb5365b26b7ab))

## [0.3.7](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.3.6...@lion/radio-group@0.3.7) (2019-12-02)

### Bug Fixes

- use strict versions to get correct deps on older versions ([8645c13](https://github.com/ing-bank/lion/commit/8645c13b1d77e488713f2e5e0e4e00c4d30ea1ee))

## [0.3.6](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.3.5...@lion/radio-group@0.3.6) (2019-12-01)

**Note:** Version bump only for package @lion/radio-group

## [0.3.5](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.3.4...@lion/radio-group@0.3.5) (2019-11-28)

**Note:** Version bump only for package @lion/radio-group

## [0.3.4](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.3.3...@lion/radio-group@0.3.4) (2019-11-27)

**Note:** Version bump only for package @lion/radio-group

## [0.3.3](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.3.2...@lion/radio-group@0.3.3) (2019-11-27)

**Note:** Version bump only for package @lion/radio-group

## [0.3.2](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.3.1...@lion/radio-group@0.3.2) (2019-11-26)

**Note:** Version bump only for package @lion/radio-group

## [0.3.1](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.3.0...@lion/radio-group@0.3.1) (2019-11-22)

**Note:** Version bump only for package @lion/radio-group

# [0.3.0](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.2.1...@lion/radio-group@0.3.0) (2019-11-18)

### Features

- finalize validation and adopt it everywhere ([396deb2](https://github.com/ing-bank/lion/commit/396deb2e3b4243f102a5c98e9b0518fa0f31a6b1))

## [0.2.1](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.2.0...@lion/radio-group@0.2.1) (2019-11-15)

**Note:** Version bump only for package @lion/radio-group

# [0.2.0](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.76...@lion/radio-group@0.2.0) (2019-11-13)

### Features

- remove all deprecations from lion ([66d3d39](https://github.com/ing-bank/lion/commit/66d3d390aebeaa61b6effdea7d5f7eea0e89c894))

## [0.1.76](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.75...@lion/radio-group@0.1.76) (2019-11-12)

**Note:** Version bump only for package @lion/radio-group

## [0.1.75](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.74...@lion/radio-group@0.1.75) (2019-11-06)

**Note:** Version bump only for package @lion/radio-group

## [0.1.74](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.73...@lion/radio-group@0.1.74) (2019-11-01)

### Bug Fixes

- **fieldset:** manage when to show error messages ([c984a66](https://github.com/ing-bank/lion/commit/c984a66))

## [0.1.73](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.72...@lion/radio-group@0.1.73) (2019-10-25)

### Bug Fixes

- **radio-group:** change check of value to only null or undefined ([fd98a55](https://github.com/ing-bank/lion/commit/fd98a55))

## [0.1.72](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.71...@lion/radio-group@0.1.72) (2019-10-25)

**Note:** Version bump only for package @lion/radio-group

## [0.1.71](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.70...@lion/radio-group@0.1.71) (2019-10-23)

**Note:** Version bump only for package @lion/radio-group

## [0.1.70](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.69...@lion/radio-group@0.1.70) (2019-10-23)

**Note:** Version bump only for package @lion/radio-group

## [0.1.69](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.68...@lion/radio-group@0.1.69) (2019-10-21)

**Note:** Version bump only for package @lion/radio-group

## [0.1.68](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.67...@lion/radio-group@0.1.68) (2019-10-14)

**Note:** Version bump only for package @lion/radio-group

## [0.1.67](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.66...@lion/radio-group@0.1.67) (2019-10-11)

**Note:** Version bump only for package @lion/radio-group

## [0.1.66](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.65...@lion/radio-group@0.1.66) (2019-10-11)

**Note:** Version bump only for package @lion/radio-group

## [0.1.65](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.64...@lion/radio-group@0.1.65) (2019-10-09)

**Note:** Version bump only for package @lion/radio-group

## [0.1.64](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.63...@lion/radio-group@0.1.64) (2019-10-07)

**Note:** Version bump only for package @lion/radio-group

## [0.1.63](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.62...@lion/radio-group@0.1.63) (2019-09-30)

**Note:** Version bump only for package @lion/radio-group

## [0.1.62](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.61...@lion/radio-group@0.1.62) (2019-09-27)

**Note:** Version bump only for package @lion/radio-group

## [0.1.61](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.60...@lion/radio-group@0.1.61) (2019-09-25)

**Note:** Version bump only for package @lion/radio-group

## [0.1.60](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.59...@lion/radio-group@0.1.60) (2019-09-20)

**Note:** Version bump only for package @lion/radio-group

## [0.1.59](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.58...@lion/radio-group@0.1.59) (2019-09-19)

**Note:** Version bump only for package @lion/radio-group

## [0.1.58](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.57...@lion/radio-group@0.1.58) (2019-09-17)

### Bug Fixes

- **lion-radio-group:** handle unchecked state ([1adeb46](https://github.com/ing-bank/lion/commit/1adeb46))

## [0.1.57](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.56...@lion/radio-group@0.1.57) (2019-09-13)

**Note:** Version bump only for package @lion/radio-group

## [0.1.56](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.55...@lion/radio-group@0.1.56) (2019-08-23)

**Note:** Version bump only for package @lion/radio-group

## [0.1.55](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.54...@lion/radio-group@0.1.55) (2019-08-21)

**Note:** Version bump only for package @lion/radio-group

## [0.1.54](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.53...@lion/radio-group@0.1.54) (2019-08-17)

**Note:** Version bump only for package @lion/radio-group

## [0.1.53](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.52...@lion/radio-group@0.1.53) (2019-08-15)

**Note:** Version bump only for package @lion/radio-group

## [0.1.52](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.51...@lion/radio-group@0.1.52) (2019-08-15)

**Note:** Version bump only for package @lion/radio-group

## [0.1.51](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.50...@lion/radio-group@0.1.51) (2019-08-14)

**Note:** Version bump only for package @lion/radio-group

## [0.1.50](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.49...@lion/radio-group@0.1.50) (2019-08-07)

**Note:** Version bump only for package @lion/radio-group

## [0.1.49](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.48...@lion/radio-group@0.1.49) (2019-08-07)

**Note:** Version bump only for package @lion/radio-group

## [0.1.48](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.47...@lion/radio-group@0.1.48) (2019-07-30)

**Note:** Version bump only for package @lion/radio-group

## [0.1.47](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.46...@lion/radio-group@0.1.47) (2019-07-30)

**Note:** Version bump only for package @lion/radio-group

## [0.1.46](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.45...@lion/radio-group@0.1.46) (2019-07-29)

**Note:** Version bump only for package @lion/radio-group

## [0.1.45](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.44...@lion/radio-group@0.1.45) (2019-07-25)

**Note:** Version bump only for package @lion/radio-group

## [0.1.44](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.43...@lion/radio-group@0.1.44) (2019-07-24)

**Note:** Version bump only for package @lion/radio-group

## [0.1.43](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.42...@lion/radio-group@0.1.43) (2019-07-24)

**Note:** Version bump only for package @lion/radio-group

## [0.1.42](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.41...@lion/radio-group@0.1.42) (2019-07-23)

**Note:** Version bump only for package @lion/radio-group

## [0.1.41](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.40...@lion/radio-group@0.1.41) (2019-07-23)

**Note:** Version bump only for package @lion/radio-group

## [0.1.40](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.39...@lion/radio-group@0.1.40) (2019-07-23)

**Note:** Version bump only for package @lion/radio-group

## [0.1.39](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.38...@lion/radio-group@0.1.39) (2019-07-22)

**Note:** Version bump only for package @lion/radio-group

## [0.1.38](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.37...@lion/radio-group@0.1.38) (2019-07-19)

**Note:** Version bump only for package @lion/radio-group

## [0.1.37](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.36...@lion/radio-group@0.1.37) (2019-07-19)

**Note:** Version bump only for package @lion/radio-group

## [0.1.36](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.35...@lion/radio-group@0.1.36) (2019-07-18)

**Note:** Version bump only for package @lion/radio-group

## [0.1.35](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.34...@lion/radio-group@0.1.35) (2019-07-17)

**Note:** Version bump only for package @lion/radio-group

## [0.1.34](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.33...@lion/radio-group@0.1.34) (2019-07-16)

**Note:** Version bump only for package @lion/radio-group

## [0.1.33](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.32...@lion/radio-group@0.1.33) (2019-07-16)

**Note:** Version bump only for package @lion/radio-group

## [0.1.32](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.31...@lion/radio-group@0.1.32) (2019-07-15)

**Note:** Version bump only for package @lion/radio-group

## [0.1.31](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.30...@lion/radio-group@0.1.31) (2019-07-15)

**Note:** Version bump only for package @lion/radio-group

## [0.1.30](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.29...@lion/radio-group@0.1.30) (2019-07-09)

**Note:** Version bump only for package @lion/radio-group

## [0.1.29](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.28...@lion/radio-group@0.1.29) (2019-07-04)

**Note:** Version bump only for package @lion/radio-group

## [0.1.28](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.27...@lion/radio-group@0.1.28) (2019-07-02)

**Note:** Version bump only for package @lion/radio-group

## [0.1.27](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.26...@lion/radio-group@0.1.27) (2019-07-02)

**Note:** Version bump only for package @lion/radio-group

## [0.1.26](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.25...@lion/radio-group@0.1.26) (2019-06-27)

**Note:** Version bump only for package @lion/radio-group

## [0.1.25](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.24...@lion/radio-group@0.1.25) (2019-06-25)

**Note:** Version bump only for package @lion/radio-group

## [0.1.24](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.23...@lion/radio-group@0.1.24) (2019-06-24)

**Note:** Version bump only for package @lion/radio-group

## [0.1.23](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.22...@lion/radio-group@0.1.23) (2019-06-20)

**Note:** Version bump only for package @lion/radio-group

## [0.1.22](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.21...@lion/radio-group@0.1.22) (2019-06-18)

**Note:** Version bump only for package @lion/radio-group

## [0.1.21](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.20...@lion/radio-group@0.1.21) (2019-06-06)

**Note:** Version bump only for package @lion/radio-group

## [0.1.20](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.19...@lion/radio-group@0.1.20) (2019-06-04)

**Note:** Version bump only for package @lion/radio-group

## [0.1.19](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.18...@lion/radio-group@0.1.19) (2019-05-31)

**Note:** Version bump only for package @lion/radio-group

## [0.1.18](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.17...@lion/radio-group@0.1.18) (2019-05-31)

**Note:** Version bump only for package @lion/radio-group

## [0.1.17](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.16...@lion/radio-group@0.1.17) (2019-05-29)

**Note:** Version bump only for package @lion/radio-group

## [0.1.16](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.15...@lion/radio-group@0.1.16) (2019-05-29)

**Note:** Version bump only for package @lion/radio-group

## [0.1.15](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.14...@lion/radio-group@0.1.15) (2019-05-24)

**Note:** Version bump only for package @lion/radio-group

## [0.1.14](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.13...@lion/radio-group@0.1.14) (2019-05-22)

**Note:** Version bump only for package @lion/radio-group

## [0.1.13](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.12...@lion/radio-group@0.1.13) (2019-05-21)

**Note:** Version bump only for package @lion/radio-group

## [0.1.12](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.11...@lion/radio-group@0.1.12) (2019-05-17)

**Note:** Version bump only for package @lion/radio-group

## [0.1.11](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.10...@lion/radio-group@0.1.11) (2019-05-16)

**Note:** Version bump only for package @lion/radio-group

## [0.1.10](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.9...@lion/radio-group@0.1.10) (2019-05-16)

**Note:** Version bump only for package @lion/radio-group

## [0.1.9](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.8...@lion/radio-group@0.1.9) (2019-05-15)

**Note:** Version bump only for package @lion/radio-group

## [0.1.8](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.7...@lion/radio-group@0.1.8) (2019-05-13)

**Note:** Version bump only for package @lion/radio-group

## [0.1.7](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.6...@lion/radio-group@0.1.7) (2019-05-13)

### Bug Fixes

- add prepublish step to make links absolute for npm docs ([9f2c4f6](https://github.com/ing-bank/lion/commit/9f2c4f6))

## [0.1.6](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.5...@lion/radio-group@0.1.6) (2019-05-08)

**Note:** Version bump only for package @lion/radio-group

## [0.1.5](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.4...@lion/radio-group@0.1.5) (2019-05-07)

**Note:** Version bump only for package @lion/radio-group

## [0.1.4](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.3...@lion/radio-group@0.1.4) (2019-04-29)

**Note:** Version bump only for package @lion/radio-group

## [0.1.3](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.2...@lion/radio-group@0.1.3) (2019-04-28)

### Bug Fixes

- update storybook/linting; adjust story labels, eslint ignores ([8d96f84](https://github.com/ing-bank/lion/commit/8d96f84))

## [0.1.2](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.1...@lion/radio-group@0.1.2) (2019-04-27)

**Note:** Version bump only for package @lion/radio-group

## [0.1.1](https://github.com/ing-bank/lion/compare/@lion/radio-group@0.1.0...@lion/radio-group@0.1.1) (2019-04-26)

### Bug Fixes

- add missing files to npm packages ([0e3ca17](https://github.com/ing-bank/lion/commit/0e3ca17))

# 0.1.0 (2019-04-26)

### Features

- release inital public lion version ([ec8da8f](https://github.com/ing-bank/lion/commit/ec8da8f))
