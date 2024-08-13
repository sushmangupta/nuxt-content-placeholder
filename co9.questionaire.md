---
questions:
# 1st question
  - question: "Before performing a Shopware update, what is a crucial step to ensure data integrity?"
    answers:
    - "Install new plugins"
    - "Disable all themes"
    - "Backup your existing data"
    - "Clear the cache"
    correct: Backup your existing data

# 2nd question
  - question: "What is the primary purpose of a patch release in Shopware?"
    answers:
    - "To introduce new features"
    - "To perform critical fixes or address security vulnerabilities"
    - "To remove deprecated code"
    - "To enhance website design"
    correct: "To perform critical fixes or address security vulnerabilities"

# 3rd question
    - question: "Your Shopware store has been heavily customized, including numerous custom themes, plugins, and integrations. A major update is available that promises improved performance and new features that you want to leverage.How would you prepare your store for this major update to ensure a smooth transition with minimal downtime?"
    answers:
    - Update the store directly in the live environment to save time.
    - First, create a backup, test the update in a staging environment, check plugin compatibility, and then deploy during off-peak hours.
    - Disable all custom plugins before updating and re-enable them afterward.
    - Skip the major update and wait for the next minor release.
    correct: "First...."

# 4th question
    - question: "A critical security vulnerability has been identified in your current Shopware version. The Shopware team has released a patch to address this issue. Your store is experiencing high traffic, and downtime must be minimized.How would you approach applying this patch to ensure your store remains secure while minimizing disruption to your customers?"
    answers:
    - "Apply the patch immediately in the live environment without taking a backup."
    - "Schedule the patch update during a low-traffic period, take a backup, and monitor the store after applying the patch."
    - "Wait until the traffic decreases naturally, then apply the patch without a backup."
    - "Ignore the patch if the store is running fine and revisit it later."
    correct: "schedule...."

#5th question
    - question: "You initiated a Shopware update using composer update, but the process was interrupted, leaving your store in an unstable state. Customers are reporting issues with accessing the website.What steps would you take to quickly restore normal operations?"
    answers:
    - "Re-run the update command in the live environment immediately."
    - "Identify the issue, attempt a rollback using the backup, and if needed, restore the store from the backup."
    - "Identify the issue, attempt a rollback using the backup, and if needed, restore the store from the backup."
    - "Identify the issue, attempt a rollback using the backup, and if needed, restore the store from the backup."
    correct: "2nd option"

#6th question
    - question: "A new minor release has introduced features that your marketing team is eager to use. However, you also rely on a third-party plugin that hasn’t yet confirmed compatibility with the new release.What process would you follow to update Shopware to this minor release, considering the potential plugin compatibility issue?"
    answers:
    - "Immediately apply the update to take advantage of the new features, then deal with any plugin issues afterward."
    - "Wait until the third-party plugin confirms compatibility, then apply the update directly to the live store."
    - "Test the update in a staging environment, check plugin compatibility, and update during a low-traffic period."
    - "Disable the third-party plugin, apply the update, and re-enable the plugin later."
    correct: "3rd option"


---