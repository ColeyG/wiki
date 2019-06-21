# Self Code Review Checklist

The following is a checklist to be completed before any MRs are submitted to another dev for review.

## General

- [] Is the MR not marked as WIP?
- [] Is the MR description correct & concise?
- [] Did the MR pass all pipelines?
- [] Check Doc Blocks/type hinting
  - [] Are _all_ comitted doc blocks correct?
  - [] Do any of them need to change from associated commited changes?
- [] Are there no MR conflicts?
- [] Are the applicable tests completed?
  - Testing on certain browsers etc

## All Code

- [] Take a moment to think about future proofing
  - [] Are there no multiple instantiations of the same functionality?
    - Can they be "variablized" or "functionized"?
- [] Are any files unintentionally changed?
  - Check every file for changes made, did you make them?
- Are dependencies up to date locally? Compiling with older versions or packages could lead to wierd changes

## Magento 2

- [] Will config have changed?
  - Have you added or disabled any modules?
- [] Does composer need updating?
  - Do you have composer.json in any new modules?
  - Have you imported any new modules?
- [] Check localizations & escapes
  - [] For **ALL** text
  - [] Is there things in translations that shouldn't be?
- [] Do all template.phtml files have doc blocks?

## Sass

- [] Is it linted?
- [] Did you check using the review task?
- [] Are there no direct css values?
  - [] Values should be calculated using rem calc etc.
