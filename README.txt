MINI&ME FOOTBALL CLUB PROJECT README Stable Baseline: v2.12.0 Date: 17
August 2026

1.  PROJECT STATUS

Mini&Me Football Club has reached its first formal stable baseline at
v2.12.0.

The game is a local, browser-based football management simulation built
as a self-contained HTML application. Development to this point has
focused on establishing the complete playable career loop, domestic and
international football systems, long-term career progression, data
persistence, and a mobile-friendly management interface.

From v2.12.0 onward, the development priority is refinement rather than
major feature expansion. Future updates should primarily address:

• Bugs and save-state issues. • AI behaviour and simulation realism. •
Match and competition logic. • UX, UI and GUI improvements. • Data
accuracy, clarity and presentation. • Performance and responsiveness. •
Compatibility with existing saves where practical.

New major systems should only be introduced where they materially
improve the existing game.

2.  CURRENT STABLE BUILD

File: MiniMe_Football_v2_12_0_StableBaseline.html

Version: v2.12.0 Stable Baseline

This build should be treated as the reference point for all subsequent
development. Earlier builds remain useful for historical comparison but
should not be used as the development baseline unless specifically
required for regression testing.

3.  CURRENT GAME SCOPE

The stable game includes:

• Multi-season football management careers. • Domestic league and cup
competitions. • Squad management, contracts and player development. •
Transfer market and recruitment. • Club records, history, statistics and
honours. • GM profile, reputation and career progression. • Club and
football-world news. • International club competition. • National team
management. • International friendlies and World Cup qualification. •
Confederation-based World Cup qualification. • 32-team World Cup with
group and knockout stages. • World Cup qualification tables and status
tracking. • World Cup season-review snapshots. • International player
appearances and career records. • Nation-strength simulation logic. •
Persistent career saves.

4.  NATIONAL TEAM AND WORLD CUP MODEL

The international system now uses a separate nation-strength model to
improve realism.

Nation strength tiers are internal engine data only. They are not
displayed to the player. They are used to help ensure established
football powers remain appropriately strong while still allowing
credible upsets and long-term variation.

The system is intended to make nations such as Brazil, France,
Argentina, Germany, Spain, Italy and other established powers
consistently competitive without making results predetermined.

Regional powers are also recognised within their confederations,
including nations such as Australia, Japan and South Korea in the AFC,
and the United States and Mexico in CONCACAF.

Lower-ranked nations can qualify for major tournaments and produce
occasional strong runs, but these should be exceptional rather than
routine.

5.  NATIONAL TEAM MANAGEMENT

As of v2.12.0, national team management is designed to work even when
the GM does not manually intervene.

The AI automatically selects a balanced 23-player national squad and
best-fit starting XI from eligible players.

The GM may review the squad and override AI selections by removing
players and calling up alternatives. Manual selections become an
explicit GM override.

If the GM does nothing, the AI-selected squad remains valid and the
national team continues normally. National management should therefore
be an optional layer of control rather than a mandatory administrative
task.

National-team notifications should only appear when the GM’s nation has
a genuine upcoming fixture or tournament requirement.

6.  WORLD CUP QUALIFICATION

World Cup qualification is tracked by federation and should reflect the
allocated places for the 32-team tournament.

Qualification screens are intended to show:

• Confederation and qualification year. • Group or league tables. •
Matches played. • Goal difference. • Points. • Qualification status such
as Qualified, Eliminated, Playoff or still active. • Wider qualification
progress so the player can follow nations outside their own federation.

Qualification tables should represent the actual saved competition state
and should not display obsolete tables from previous World Cup cycles.

7.  WORLD CUP

The World Cup uses a 32-team structure with:

• Eight groups. • Group-stage fixtures and tables. • Progression into
knockout rounds. • Round of 16. • Quarter-finals. • Semi-finals. •
Third-place match. • Final. • Tournament champion and historical review
data.

Domestic league football is paused during the active World Cup
tournament period so the tournament can progress as its own major event.

8.  SIMULATION PHILOSOPHY

Domestic club football and international football should not be assumed
to use identical simulation behaviour.

International results need to account for national-team strength and the
greater historical stability of international football hierarchies.

Large upsets remain possible, but repeated implausible results or
tournament runs by substantially weaker nations should be treated as
simulation issues requiring tuning.

The goal is credible unpredictability, not pure randomness.

9.  DEVELOPMENT TOOLS

The temporary developer Quick Sim feature has been removed and disabled
in v2.12.0.

The stable player-facing build should not expose development-only
controls.

Where future testing tools are required, they should preferably be
isolated from the normal player interface or maintained in a separate
development build.

10. SAVE COMPATIBILITY

The game has undergone substantial international-system development
across multiple versions.

Legacy careers may contain historical competition state created under
older World Cup or qualification logic. Compatibility and migration
safeguards have been added where practical, but old saves can still
expose data that would not occur in a newly created v2.12.0 career.

When assessing a suspected simulation bug, test against a new v2.12.0
career where possible before determining whether the issue is current
logic or legacy save data.

Existing saves should not be deliberately broken by future updates
without a strong reason.

11. DEVELOPMENT PRINCIPLES FROM v2.12.0

The stable baseline should be protected.

Changes should be incremental, testable and versioned.

Priority order:

1.  Fix reproducible bugs.

2.  Protect save integrity.

3.  Improve simulation and AI behaviour.

4.  Improve gameplay logic.

5.  Improve displayed information and clarity.

6.  Improve UX and navigation.

7.  Improve UI and GUI presentation.

8.  Improve performance.

9.  Add new functionality only where it clearly strengthens the existing
    game.

10. VERSIONING

v2.12.0 is the Stable Baseline.

Recommended version approach:

v2.12.x Maintenance, bug fixes, AI tuning, UX/UI improvements and minor
functional refinements.

v2.13.0 and later Meaningful feature or system improvements that extend
the stable game without redefining its architecture.

Major version changes should be reserved for substantial changes to the
game structure or underlying architecture.

13. TESTING PRIORITIES

Future builds should be checked for:

• New Career and Load Career. • Save persistence after reload. • Season
progression. • Domestic league and cup progression. • Promotion and
relegation. • Transfers and contract changes. • Player development. •
International windows. • National squad AI selection. • Manual national
squad overrides. • World Cup qualification progression. • Confederation
table accuracy. • Qualification status accuracy. • World Cup group and
knockout progression. • International result realism. • Season Review
accuracy. • Historical records. • Mobile layout. • Desktop layout. •
Navigation and button routing. • Legacy save behaviour where relevant.

14. REPOSITORY RECOMMENDATION

Suggested core repository files:

README.txt This project overview and stable-baseline record.

CHANGELOG.txt A concise chronological record of released versions and
changes.

TESTING_CHECKLIST.txt A repeatable regression checklist for future
builds.

MiniMe_Football_v2_12_0_StableBaseline.html The current stable game.

Older release files may be retained in a Releases or Archive folder
rather than alongside the current stable build.

15. CURRENT DIRECTION

Mini&Me Football Club is now considered feature-complete enough to move
into a sustained refinement phase.

The objective is no longer to continuously expand the number of systems.
The objective is to make the systems already present increasingly
reliable, believable, intuitive and polished.

Stable Baseline: Mini&Me Football Club v2.12.0 17 August 2026
