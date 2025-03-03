# Bug Bounty

Participate in the Safe Bug Bounty program to find bugs and get rewards. Earn up to $1,000,000 for every bug you report. Please carefully read through the [submission process](./bug-bounty-program.md#submission-process) section and get in touch via [bounty@safe.global](mailto:bounty@safe.global). You can also review the [bug bounties](./past-paid-bounties.md) we have paid in the past.

## Audits

Smart contract security experts have carefully audited Safe's contracts. Please refer to the [security audits page](./security-audits.md) for details.

## Rules

Many of the [Ethereum Foundation's bug bounty program rules](https://bounty.ethereum.org) are also applicable to the Safe Bug Bounty program:

* Issues already submitted by another user or known to the Safe team are not eligible for bounty rewards.
* Public disclosure of a vulnerability makes it ineligible for a bounty.
* The Safe core development team, employees, and all other people paid by Safe, directly or indirectly (including the external auditors), are not eligible for rewards.
* The Safe Bounty program considers several variables in determining rewards. Determinations of eligibility, score, and all terms related to an award are at the sole and final discretion of the Safe Bug Bounty panel.

## Scope

The scope of the bug bounty program includes the core contracts related to the following releases of the Safe contracts:

* v1.4.1 ([Release details](https://github.com/safe-global/safe-contracts/releases/tag/v1.4.1), [readme](https://github.com/safe-global/safe-contracts/blob/v1.4.1/README.md))
* _v1.3.0_ ([Release details](https://github.com/safe-global/safe-contracts/releases/tag/v1.3.0), [readme](https://github.com/safe-global/safe-contracts/blob/v1.3.0/README.md))
* _v1.2.0_ ([Release details](https://github.com/safe-global/safe-contracts/releases/tag/v1.2.0), [readme](https://github.com/safe-global/safe-contracts/blob/v1.2.0/README.md))
* _v1.1.1_ ([Release details](https://github.com/safe-global/safe-contracts/releases/tag/v1.1.1), [readme](https://github.com/safe-global/safe-contracts/blob/v1.1.1/README.md))

The scope of the bug bounty also includes the [Allowance Module](https://github.com/safe-global/safe-modules/blob/47e2b486b0b31d97bab7648a3f76de9038c6e67b/allowances).

### In scope

**Safe core contracts (version 1.4.1)**

* Safe.sol (formerly GnosisSafe.sol)
* SafeL2.sol (formerly GnosisSafeL2.sol)
* SafeProxyFactory.sol (formerly GnosisSafeProxyFactory.sol)
* SafeProxy.sol (formerly GnosisSafeProxy.sol)
* MultiSend.sol, MultiSendCallOnly.sol, CreateCall.sol
* TokenCallbackHandler.sol (formerly DefaultCallbackHandler.sol), CompatibilityFallbackHandler.sol, HandlerContext.sol

You can find addresses for deployed instances of these contracts in the [Safe deployments](https://github.com/safe-global/safe-deployments) repository.

**Gnosis Safe core contracts (up to version 1.3.0)**

* GnosisSafe.sol
* GnosisSafeL2.sol
* GnosisSafeProxyFactory.sol (formerly ProxyFactory.sol)
* GnosisSafeProxy.sol (formerly Proxy.sol)
* CreateAndAddModules.sol, MultiSend.sol, MultiSendCallOnly.sol, CreateCall.sol
* DefaultCallbackHandler.sol, CompatibilityFallbackHandler.sol, HandlerContext.sol

You can find addresses for deployed instances of these contracts in the [Safe deployments](https://github.com/safe-global/safe-deployments) repository.

**Safe Modules contracts**

* AllowanceModule.sol

### Examples of what's in scope

* Being able to steal funds
* Being able to freeze funds or render them inaccessible by their owners
* Being able to perform replay attacks on the same chain
* Being able to change Safe settings or module settings without the consent of owners

### Out of scope

* Any files, Safe Modules, or libraries other than the ones mentioned above
* More efficient gas solutions
* Any points listed as an already known weaknesses
* Any points listed in the audit or formal verification results reports
* Any points fixed in a newer version

## Intended behavior

Please refer to the [readme file](https://github.com/safe-global/safe-contracts/blob/v1.3.0/README.md) and the [release details](https://github.com/safe-global/safe-contracts/releases) of the respective contract version on GitHub as well as our [developer docs](https://docs.safe.global) for an extensive overview of the intended behavior of the smart contracts.

For the allowance module, please refer to the corresponding [README file](https://github.com/safe-global/safe-modules/blob/47e2b486b0b31d97bab7648a3f76de9038c6e67b/allowances/README.md).

## Compensation

All bugs (they do not necessarily need to lead to a redeploy) will be considered for a bounty, but the severity of the threat will change the reward. Below are the reward levels for each threat severity and an example of such a threat.

### High threat: up to $1,000,000

An identified attack that could steal funds or tokens or lock user funds would be considered a high threat. Likewise, a reported bug that, on its own, leads to a redeploy of the code will always be regarded as a high threat.

### Medium threat: up to $50,000

An identified attack where it is possible to steal funds because of unexpected behavior on the user's part. Unexpected behavior here means the user can't anticipate and comprehend that they will lose the funds.

### Low threat: up to $10,000

A way to avoid transaction fees or an exploit that in some way compromises the experience of other Safe users.

_Safe will pay all bounties in ETH._

Please note that the submission's quality will factor into the level of compensation. A high-quality submission should include an explanation of how somebody can reproduce the bug.


## Submission Process

Please email your submissions to [bounty@safe.global](mailto:bounty@safe.global).

Remember to include your ETH address so that you may be rewarded. If more than one address is specified, Safe will use only one at the discretion of the bounty program administrators. Anonymous submissions are welcome, too.

Please consult our [privacy policy](https://safe.global/privacy) for further details on how we handle submissions.

## Responsible Disclosure Policy

If you comply with the policies below when reporting a security issue to us, we will not initiate a lawsuit or law enforcement investigation against you in response to your report.

_We ask that:_

* You give us reasonable time to investigate and mitigate an issue you report before making public any information about the report or sharing such information with others.
* You make a good faith effort to avoid privacy violations and disruptions to others, including (but not limited to) data destruction and interruption or degradation of our services.
* You do not exploit a security issue you discover for any reason. This includes demonstrating additional risk, such as an attempted compromise of sensitive company data or probing for additional issues.
* You do not violate any other applicable laws or regulations.

Public disclosure of the bug or the indication of an intention to exploit it on Mainnet will make the report ineligible for a bounty. If in doubt about other aspects of the bounty, most of the [Ethereum Foundation bug bounty program rules](https://bounty.ethereum.org) will apply here.

Any questions? Reach us via email ([bounty@safe.global](mailto:bounty@safe.global)) or [Discord](https://chat.safe.global). For more information on the Safe, check out our [website](https://safe.global) and our [GitHub](https://github.com/safe-global).

_Happy hunting!_
