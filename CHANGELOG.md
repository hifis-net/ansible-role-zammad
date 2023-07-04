# Changelog

## [v2.0.0](https://github.com/hifis-net/ansible-role-zammad/tree/v2.0.0) (2023-07-04)

[Full Changelog](https://github.com/hifis-net/ansible-role-zammad/compare/1.4.0...v2.0.0)

**Implemented enhancements:**

- feat: ensure compatibility with Zammad \>= 6.0 [\#37](https://github.com/hifis-net/ansible-role-zammad/pull/37) ([tobiashuste](https://github.com/tobiashuste))
- feat: add support for Ubuntu 22.04 [\#34](https://github.com/hifis-net/ansible-role-zammad/pull/34) ([tobiashuste](https://github.com/tobiashuste))

**Closed issues:**

- Add CITATION.cff [\#39](https://github.com/hifis-net/ansible-role-zammad/issues/39)
- Establish compatibility with Zammad \>= 6.0 [\#36](https://github.com/hifis-net/ansible-role-zammad/issues/36)
- Update README [\#35](https://github.com/hifis-net/ansible-role-zammad/issues/35)
- Unify the GitHub Actions workflow with other projects [\#31](https://github.com/hifis-net/ansible-role-zammad/issues/31)
- Add CHANGELOG [\#30](https://github.com/hifis-net/ansible-role-zammad/issues/30)
- Rename default branch to main [\#29](https://github.com/hifis-net/ansible-role-zammad/issues/29)
- Add support for Ubuntu 22.04 [\#27](https://github.com/hifis-net/ansible-role-zammad/issues/27)

**Merged pull requests:**

- fix: properly check if the ssl variables are set [\#41](https://github.com/hifis-net/ansible-role-zammad/pull/41) ([tobiashuste](https://github.com/tobiashuste))
- chore: add CITATION.cff [\#40](https://github.com/hifis-net/ansible-role-zammad/pull/40) ([Normo](https://github.com/Normo))
- docs: update README information [\#38](https://github.com/hifis-net/ansible-role-zammad/pull/38) ([tobiashuste](https://github.com/tobiashuste))
- style: fix ansible-lint violations [\#33](https://github.com/hifis-net/ansible-role-zammad/pull/33) ([tobiashuste](https://github.com/tobiashuste))
- ci: fix and align GitHub Actions workflow [\#32](https://github.com/hifis-net/ansible-role-zammad/pull/32) ([tobiashuste](https://github.com/tobiashuste))
- ci: configure Dependabot version updates [\#28](https://github.com/hifis-net/ansible-role-zammad/pull/28) ([tobiashuste](https://github.com/tobiashuste))
- Bump geerlingguy.postgresql from 2.2.1 to 3.0.0 [\#26](https://github.com/hifis-net/ansible-role-zammad/pull/26) ([Normo](https://github.com/Normo))
- Set Zammad 3.6.0 as default version [\#25](https://github.com/hifis-net/ansible-role-zammad/pull/25) ([Normo](https://github.com/Normo))
- Bump elastic.elasticsearch from 7.9.3 to 7.10.0 [\#24](https://github.com/hifis-net/ansible-role-zammad/pull/24) ([Normo](https://github.com/Normo))

## [1.4.0](https://github.com/hifis-net/ansible-role-zammad/tree/1.4.0) (2020-11-09)

[Full Changelog](https://github.com/hifis-net/ansible-role-zammad/compare/1.3.0...1.4.0)

**Implemented enhancements:**

- Add Ansible Galaxy release job [\#23](https://github.com/hifis-net/ansible-role-zammad/pull/23) ([Normo](https://github.com/Normo))

**Closed issues:**

- Automate role import into Ansible Galaxy [\#19](https://github.com/hifis-net/ansible-role-zammad/issues/19)

**Merged pull requests:**

- Bump elastic.elasticsearch from 7.9.2 to 7.9.3 [\#22](https://github.com/hifis-net/ansible-role-zammad/pull/22) ([Normo](https://github.com/Normo))
- Update molecule action [\#21](https://github.com/hifis-net/ansible-role-zammad/pull/21) ([Normo](https://github.com/Normo))
- Explicitly set file permissions for repository files [\#20](https://github.com/hifis-net/ansible-role-zammad/pull/20) ([Normo](https://github.com/Normo))

## [1.3.0](https://github.com/hifis-net/ansible-role-zammad/tree/1.3.0) (2020-10-06)

[Full Changelog](https://github.com/hifis-net/ansible-role-zammad/compare/1.2.0...1.3.0)

**Implemented enhancements:**

- Allow to disable Nginx version information [\#15](https://github.com/hifis-net/ansible-role-zammad/issues/15)
- Allow to specify SSL certificates via path only [\#13](https://github.com/hifis-net/ansible-role-zammad/issues/13)

**Merged pull requests:**

- Bump elastic.elasticsearch from 7.9.0 to 7.9.2 [\#18](https://github.com/hifis-net/ansible-role-zammad/pull/18) ([tobiashuste](https://github.com/tobiashuste))
- Install Zammad 3.5.0 by default [\#17](https://github.com/hifis-net/ansible-role-zammad/pull/17) ([tobiashuste](https://github.com/tobiashuste))
- Allow to configure nginx server\_tokens directive [\#16](https://github.com/hifis-net/ansible-role-zammad/pull/16) ([tobiashuste](https://github.com/tobiashuste))
- Allow to use SSL keypair given by path only [\#14](https://github.com/hifis-net/ansible-role-zammad/pull/14) ([tobiashuste](https://github.com/tobiashuste))

## [1.2.0](https://github.com/hifis-net/ansible-role-zammad/tree/1.2.0) (2020-08-27)

[Full Changelog](https://github.com/hifis-net/ansible-role-zammad/compare/1.1.0...1.2.0)

**Implemented enhancements:**

- Add Ubuntu 20.04 focal support [\#8](https://github.com/hifis-net/ansible-role-zammad/issues/8)
- Allow to optionally configure additional server directives in Nginx config [\#5](https://github.com/hifis-net/ansible-role-zammad/issues/5)
- Allow to optionally configure additional Nginx server directives [\#7](https://github.com/hifis-net/ansible-role-zammad/pull/7) ([tobiashuste](https://github.com/tobiashuste))

**Merged pull requests:**

- molecule verify: Check wether Zammad web interface is available [\#12](https://github.com/hifis-net/ansible-role-zammad/pull/12) ([Normo](https://github.com/Normo))
- Add Ubuntu 20.4 support [\#11](https://github.com/hifis-net/ansible-role-zammad/pull/11) ([Normo](https://github.com/Normo))
- Update molecule action [\#10](https://github.com/hifis-net/ansible-role-zammad/pull/10) ([Normo](https://github.com/Normo))
- Update requirements.yml [\#9](https://github.com/hifis-net/ansible-role-zammad/pull/9) ([Normo](https://github.com/Normo))
- Install Zammad 3.4.0 by default [\#6](https://github.com/hifis-net/ansible-role-zammad/pull/6) ([Normo](https://github.com/Normo))

## [1.1.0](https://github.com/hifis-net/ansible-role-zammad/tree/1.1.0) (2020-07-16)

[Full Changelog](https://github.com/hifis-net/ansible-role-zammad/compare/1.0.0...1.1.0)

**Implemented enhancements:**

- Allow to install packages from the development channel [\#3](https://github.com/hifis-net/ansible-role-zammad/issues/3)

**Merged pull requests:**

- Make Zammad release channel configurable [\#4](https://github.com/hifis-net/ansible-role-zammad/pull/4) ([tobiashuste](https://github.com/tobiashuste))

## [1.0.0](https://github.com/hifis-net/ansible-role-zammad/tree/1.0.0) (2020-05-12)

[Full Changelog](https://github.com/hifis-net/ansible-role-zammad/compare/157bef1dfe6bc566f10f927ab929b3910d3ea986...1.0.0)

**Merged pull requests:**

- Specify zammad version on installation [\#2](https://github.com/hifis-net/ansible-role-zammad/pull/2) ([Normo](https://github.com/Normo))
- Create GitHub actions workflow [\#1](https://github.com/hifis-net/ansible-role-zammad/pull/1) ([Normo](https://github.com/Normo))



\* *This Changelog was automatically generated by [github_changelog_generator](https://github.com/github-changelog-generator/github-changelog-generator)*
