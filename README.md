# StorageCleanerMac Updates

This public repository hosts Sparkle update feeds and release binaries for StorageCleanerMac. Source code and the MIT license are published in [StorageCleanerMac-OpenSource](https://github.com/yangyihang96/StorageCleanerMac-OpenSource).

## 1.10.1 downloads and in-app updates

[Download 1.10.1](https://github.com/yangyihang96/StorageCleanerMacUpdates/releases/tag/v1.10.1)

- Production: `存储清理助手.app`, bundle ID `com.local.StorageCleanerMac`, feed `appcast.xml`.
- Beta: `测试版.app`, bundle ID `com.local.StorageCleanerMac.beta`, feed `appcast-beta.xml`.
- Use **工具 → 检查存储清理助手更新** to check for updates. Earlier production versions keep their existing feed. Earlier local-only betas require one manual replacement with the update-enabled beta; a feed cannot enable an updater that an old binary disables.
- The channels do not replace one another. Beta checks automatically but does not install updates automatically.

Update archives are verified with Sparkle EdDSA signatures before extraction. The public verification key remains compatible with previous production builds. Private signing keys are never published.

Current builds are Apple Development signed, not Developer ID notarized. Gatekeeper distribution approval remains unavailable, and other Macs may block opening the app. Sparkle archive verification is separate from Apple notarization. Do not lower system security settings.

Test suites were not run for this update at the user's request. GitHub Actions remains disabled; build, signing and publication checks are local. See the source repository's release record for limitations.
