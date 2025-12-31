+++
date = '2025-12-31T10:35:55-03:00'
draft = false
title = 'The Personal Finance Manager Obsidian Plugin'
image = 'andre-taissin-5OUMf1Mr5pU-unsplash.jpg'
+++

The framework behind the Personal Finance Manager plugin is a simplified manner to answer a few questions at the end of every month:
- What is my total patrimony value?
- How much money I saved this month?
- How much money I have invested?
- How much investment interest did I obtain?

By tracking these 4 metrics, I was pushed to invest more and expend less, and to have more consciousness about those expenses, and the impacts of my own investments. This helped me better than micromanaging every expense I make throughout the month, and to feel less guilty about it. If I'm reaching my saving goals, I shouldn't feel bad about buying something I want, or to expend money on something frivolous.

It is a manual ritual, yes, but it's practical and quick. It takes me around 15 minutes a month for tracking 7 assets, a salary and a few dividends. In my opinion, the manual nature of it changes the way we look at the results, and make the user more aware of what is happening in their finances.

If you instead are looking for a tool that could answer where you are expending more money, or how you can improve your investment yield, you probably should look somewhere else. But instead If you are trying to set saving goals or to keep track of your patrimony, this should do the job.

I hope it helps you as much as it helped me in the last years.

## How it works

Monthly, you have to go through your assets and input the current balance. These inputs, as like all other inputs, will become .md files in your Obsidian vault. Then, you should input your transactions, which includes your salary or bonuses, and how much money you deposited or withdrew from investment assets (like investment accounts). This is enough to generate your monthly accounting file that will contain information about your total patrimony, how much money you saved, your investment interest, etc.

Optionally, you can also input reserves, which represents money you are saving for a specific future expense, like a travel, or a car, or a new TV, or if you simply want to reserve to expend in the future freely. We will explain it further about reserves in the specific session below.

To make inputs to the vault, you can use the command palette (by pressing cmd + p, or ctrl + p depending on your operational system) or the piggybank icon on the left. The commands are all preceded by a "Personal finance manager" phrase.

## The Assets

The first thing you have to setup are your assets. This can be bank accounts, digital wallets, physical safes, real estate or anything you can deposit money or financial value in it. It is important to set the right asset type, which currently are three:

1. Deposit: these are assets that won't generate interest, or the interest may be irrelevant. You don't need to register the transactions in this kind of assets, because the system understands that, since these won't generate interest, the difference of the balance between months already reflects directly the difference between incomes and outcomes. The value registered on these assets are summed to the total financial patrimony, and the total deposit patrimony in the accounting calculation.

2. Investment: these are assets that will generate passive interest, and usually they will represent accounts you have in investment agencies. It is necessary to register all deposits and withdraws in these accounts, because the difference between these deposits, withdraws and the balance between months will be used to calculate the amount of interest for those assets. It is worth mentioning that you won't need to register dividends, if these are not withdrawn from the account or if they are reinvested. Some financial agencies keep the dividends in an internal balance, and this is summed up to the total balance of the user. It is important that this internal balance is considered in the total balance for this asset. Investment assets are considered in the total financial patrimony, and the total investment patrimony calculation. The total investment interest percentage will be calculated using this total investment patrimony value.

3. Real Estate: These are useful to keep track of real estate assets. We understand that although those can gain value month by month, we don't consider this as an investment asset. The value difference will be considered only when this asset is sold, and the money is sent to other assets. You are encouraged to consider the mortgage payments and increase the value of the asset for every payment, and this is considered for your monthly savings. The purely financial saving is calculated aside from your total saving. We will discuss this further in the Patrimony session below.

## Patrimony

At the end of the month, you should register all balances from all your patrimonies. You do that by accessing the "Personal Finance Manager: Create new Patrimony Entry" command. This will open a modal where you can input the period, the asset that this balance belongs to, and the value. For each period, you can register only one patrimony entry per asset.

In case of investment patrimonies, you should consider all money invested, along with the money kept in the internal balances, that are not invested but are available to be used. If you want to, you can register the value not invested as a different deposit asset, but this will make the input process more complex, since you will need to register all money going back and forth from the internal balance to investments and the other way around. It is a trade off between complexity and accuracy, but if you don't keep lots of money on these internal balances, this should not make huge difference in the final calculus.

The Real Estate patrimony is useful to keep track of the money you save monthly in form of mortgage payment. Monthly mortgage payments usually carry an interest part along with a payment that will reduce the total debt. The interest part is a tax charged by the bank, but the mortgage reduction can be considered something that collaborates to your total patrimony.

For all effects, real estate assets are treated as a deposit asset, except that it will not sum up to the total financial patrimony value, and for the financial savings that are calculated aside from the total savings, that consider the money used to reduce the mortgage debt. You should not revaluate the real estate value every month, and differences month by month on those assets are considered as savings instead of interest. The revaluation will be done only when you sell the asset and redirect the amount you got to other assets.

As an example, if you have a $500,000 apartment and a $300,000 debt, you should consider the patrimony value as the difference, so $200,000 in this case. In the next month, you should review the debt. If your debt is then $ 298,000, the asset value should be included as $202,000. This $2000 difference is considered as a saving. If in that month you had another $1000 in financial savings, the total savings for that month will be $3000.

## Transactions

Transactions are the kind of record that will include all your incomes, like dividends, salary, bonuses, etc. and also all your deposits or withdraws in your investments. Transactions you make in your deposit assets doesn't need to be registered, since all differences month over month in those balances are enough to calculate the transactions made on them.

Transactions in your investment assets are important to be registered, since without them we couldn't calculate the correct interest. To make an example: consider an investment asset that you had $1000 in it last month. In the current month, you register a withdraw of $200 and a patrimony of $808 for that asset. The system will calculate that this asset had an interest of 1% (8 dollars). The calculation is simple: you had $1000 and withdrew $200, so it's expected that this asset had a balance of $800 this month, but instead we registered $808. The only possibility is that these $8 were interest. Since you had $800, and the interest were $8, so the percentage interest will be 8 divided by 800, so 1%.

Salaries and bonuses are important to calculate the percentage amount of savings every month. Although they are associated with an asset, this association is not important. You should never associate a bonus or a salary to an investment asset. The raw amount of savings you had in a month is calculated by the patrimony difference month over month minus the total interest. The saving percentage is calculated by dividing the total savings by the total income of bonuses and salaries. The financial savings considers the balance difference only in financial assets.

## Reserve Accounts and Reserve Transactions

Imagine you want to buy a new phone, or to pay for your vacation trip with the money you were saving for months. If you register your new patrimony balance after that big spend, you will see a big outlier in your patrimony and your savings calculations will be zero, or even negative, even though this was a calculated spend and you are still following the savings plan.

For example, imagine that you gained $1000 in a month, $500 you want to save and $500 you want to reserve to buy a new computer that costs $800. In this month, your savings will be 100%, since you didn't spend any of the money you gained. Next month, you gain another $1000, you save $700 and use the remaining $300 as a complement for the computer payment. Well, once you register all your balances, the system will calculate that you saved only $200 that month (20%), which is wrong, since you saved $700.

This is the main reason reserve accounts and reserve transactions exists. If you want to reserve part of your money to buy something in the future, you can add that money to reserve accounts. You can create as many reserve accounts as you like with particular goals, for organization purposes, but they all serve a single purpose in the end: to "pre-spend" money in a way that will allow the proper calculation of your savings.

In our example, you can create a new Reserve Account called "computer" with a goal of $800. In the first month, you register a reserve deposit of $500 in that account, that money won't be considered in your patrimony total and your savings calculation will indicate that you saved the remaining $500 (or 50%). In the next month, you may register a new transaction, now a withdraw, of $500 from that account, since you used that money to buy the computer. Your accounting will indicate that you saved $700, or 70%, which is the right value.

The "Total Patrimony" calculated in your savings won't consider the money you have reserved in your reserve accounts, but this is not the value used to calculate the Patrimony Diffs. The value used is always the "Total Net Patrimony", which considers the total amount you have in reserve. The reserve balance will also affect the Financial Patrimony and the Deposit Financial Patrimony, which will always be the "real" value minus your reserve balance. Notice that these values can be negative if for some reason the amount you have reserved is bigger than the money you have in Deposit Assets.

## Accountings

After you register all your patrimonies and transactions, you can generate the Accounting file. This file will contain all financial calculations as frontmatter properties.

Notice that this calculation considers the existing transaction and patrimony files at the moment the accounting file is created. If you create new transactions or patrimonies, you should delete the old accounting file and generate a new one to remake all calculus considering the new information.

## Configuration

In the configuration page, you can set the folders where you want to save your files. There is a specific configuration for each file type: Assets, Transactions, Patrimony entries, Reserve Accounts, Reserve Transactions and Accountings. If you change these configurations, you should manually transfer your existing files in the old location to the new one, including the internal folder structure, so all new calculations will work properly.

There is also a language configuration, which will change the configurations labels, modal names and field labels, but this won't change the field name inside the files (frontmatter), like "Value" in the Patrimony entry file. This is simply because those field names are used in the code that runs the calculation, and this would be hard to maintain. It is not as simple as just moving files around.

## Conclusion

I hope you didn't find this a complicated framework. With a few registers, like patrimonies and transactions every month, you should be able to track important indicators like total patrimony, savings, investments and interest.

Don't underestimate the power of tracking those indicators. I see myself every month eager to calculate these and check how I performed. This stimulated me to save more, invest more, and to have more grasp of my own financial health. I encourage you to give it a try and do the same.

With this small documentation you should understand all your accounting indicators. We will also include a sheet to describe them all in the next session, as an appendix.

As before mentioned, I hope this framework helps you as much as it helped me in the past years. Any feedbacks and contributions are welcome in the GitHub project page!

## Appendix: Description of the accounting indicators

*Real Estate Patrimony*: the sum of all patrimony values of type Real Estate

*Financial Patrimony*: the sum of all patrimony values of type Deposit and Investment minus the total balance of reserve accounts

*Investment Financial Patrimony*: the sum of all patrimony values of type Investment

*Deposit Financial Patrimony*: the sum of all patrimony values of type Deposit minus the total balance of reserve accounts

*Total Patrimony*: the sum of all patrimony values

*Total Net Patrimony*: the sum of all patrimony values minus the total balance of reserve accounts

*Total Income*: the sum of all transactions of type Bonus and Salary

*Total Investment Deposit*: the balance of all deposit and withdraw transactions in Investment Assets

*Total Reserve*: the sum of all balances of all reserve accounts

*Reserve Diff*: the difference between this month Total Reserve and the last month's

*Reserve Balance*: the details of balance on all reserve accounts. Do not modify this value manually.

*Patrimony Diff*: the difference between this month Total Net Patrimony and the last month's

*Financial Patrimony Diff*: the difference between this month Total Financial Patrimony and the last month's

*Investment Patrimony Diff*: the difference between this month Investment Financial Patrimony and the last month's

*Deposit Patrimony Diff*: the difference between this month Deposit Financial Patrimony and the last month's

*Real Estate Patrimony Diff*: the difference between this month Real Estate Patrimony and the last month's

*Investment Interest*: the difference between the Investment Patrimony Diff and the Total Investment Deposit, which indicates the part of the Investment Patrimony Diff not caused by investment deposits

*Percentage Investment Interest*: the Investment Interest divided by this month's Investment Financial Patrimony

*Net Economy*: the difference between the Patrimony Diff and the Investment Interest, which indicates the part of the Patrimony Diff not caused by investment interest

*Percentage Net Economy*: the Net Economy divided by this month's Total Income

*Financial Net Economy*: the difference between the Financial Patrimony Diff and the Investment Interest, which indicates the part of the Financial Patrimony Diff not caused by investment interest

*Percentage Financial Net Economy*: the Financial Net Economy divided by this month's Total Income

# Cover Image

The cover image was created by [Andre Taissin](https://unsplash.com/@andretaissin) and it's available at [Unsplash](https://unsplash.com/photos/pink-pig-coin-bank-on-brown-wooden-table-5OUMf1Mr5pU)

