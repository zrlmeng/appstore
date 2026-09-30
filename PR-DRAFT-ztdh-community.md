## Summary
- Add Docker App Store entry for 守赚开放平台·社区版 (`ztdh-community`)
- Runtime: public **enc** image only `zhitongdaohe/shouzhuan-community:1.0.2` (no business source in this pack)
- License: online activation required (`YUDAO_LICENSE_RUNTIME_ONLINE_REQUIRED=true`)
- Compose follows baota `bt_apps` labels + HOST_IP / APP_PATH conventions

## Notes for reviewers
- This is **not** PHP one-click ZIP; Docker App Store compose only
- `appid` 9101 is a placeholder — please renumber if needed
- Demo: https://install-staging.zrlmeng.com/
- Docs: https://docs.zrlmeng.com/community/

## Test plan
- [ ] `docker compose` pull + up on Baota Docker
- [ ] Open `/install` wizard
- [ ] Confirm online license activation is required
- [ ] Confirm pack contains no `.java`/`.kt` source trees

