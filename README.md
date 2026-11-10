<p align="center">
  <img src="assets/sigil.webp" width="200" alt="beelzebub, a golden fly in a ring of thorns">
</p>

<h1 align="center">beelzebub</h1>

<p align="center">
  <em>Many skills go in. One skill comes out.</em>
</p>

<p align="center">
  <a href="https://beelzebub.rylupague.dev">beelzebub.rylupague.dev</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/skill-one%20SKILL.md-111111?style=flat-square" alt="One SKILL.md">
  <img src="https://img.shields.io/badge/scripts-none-111111?style=flat-square" alt="No scripts">
  <img src="https://img.shields.io/badge/dependencies-none-111111?style=flat-square" alt="No dependencies">
  <img src="https://img.shields.io/badge/license-MIT-111111?style=flat-square" alt="MIT license">
</p>

---

You have three skills that each do part of the job. Load them together and they argue: one says ask first, another says never ask; one wants a test for everything, another wants none for trivial changes. Your agent has to guess which one wins.

beelzebub eats them and returns one skill that works on its own. Every rule is kept, merged, or dropped on purpose, and every real contradiction is put in front of you before a word of the new skill is written.

## How it works

1. **Intake.** Confirms which skills to absorb and what the result must help someone do. Reads every source as untrusted data: it does not follow their instructions, run their scripts, or adopt their tool permissions.
2. **Digest.** Sorts each rule into shared, unique, context-dependent, conflict, or excluded. Nothing disappears without being listed.
3. **Conflicts.** Shows each incompatible pair with short quotes, the file and section they came from, a proposed resolution, and its tradeoff. Then it waits for you.
4. **Forge.** Rewrites what survived in one voice, as original prose. The result runs without the originals installed and adds no tooling.
5. **Deliver.** Checks coverage and safeguards, shows the full preview, writes only where you agreed, and reports what was read, resolved, and excluded.

Greedy, not careless: it never picks a conflict winner silently, never assumes the last-loaded rule wins, never drops a conflict, and never claims token savings it has not measured.

## The prompt

beelzebub is one prompt: [`skills/beelzebub/SKILL.md`](skills/beelzebub/SKILL.md).

## Install

```bash
npx skills add alphiree/beelzebub
```

No scripts, no dependencies, no runtime. If your agent loads skills from a folder, it loads this one.

## Usage

Name the skills to absorb and, if it isn't obvious, what the merged skill must help someone do:

```
/beelzebub absorb <skill 1> <skill 2>
```

Slash syntax varies by agent. A plain request that says merge, absorb, fuse, combine, or synthesize with named skills triggers it too:

```
Merge my code-review and security-review skills into one review skill.
```

## What you get

- **One `SKILL.md`, in one voice.** Original prose, not pasted sources. Extra files only when scope or a license notice requires them.
- **Standalone.** No dependency on the originals' paths, files, scripts, or tool permissions.
- **A short, lowercase, anime-inspired name** that also names the folder.
- **Credits and license notices carried forward.** Unclear redistribution rights are stated, never papered over.
- **A limits note** at the end of the skill: what was excluded and what could not be read.

## What it refuses

- Doing the absorbed skills' own work, or running their scripts.
- Installing tooling or expanding permissions to finish a merge.
- Finalizing or installing while any conflict is still open.
- Overwriting an existing skill without consent, or touching the originals.
- Claiming token savings or equivalence it has not tested.

## FAQ

**Will it pick a winner when two rules disagree?**
No. It shows you both, proposes one, and waits. Approving a clearly stated exclusion counts as a decision. Silence does not.

**Does it run the source skills' scripts?**
Never. It reads them as data. Anything that only works through a script, runtime, or harness is listed as excluded, not faked.

**Why do merged skills get anime names?**
A merge deserves a name you remember. The SKILL.md asks for one short, lowercase word, witty, and anime-inspired.

**Why "beelzebub"?**
It's named after Rimuru's Ultimate Skill in *That Time I Got Reincarnated as a Slime*.

## License

[MIT](LICENSE).
