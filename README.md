# gogverify

Verify the installation of a game from GOG against the official MD5 hashes.

This is an unofficial tool. I am not affiliated to GOG.

I do *not* endorse piracy. This tool is intended only to verify *legally* obtained copies.

## Security

Unfortunately, only MD5 hashes are available via the GOG API, so there could theoretically be collisions.
While MD5 is (still) presumed to be resistant against preimage attacks, one can be relatively sure that no third party modified the game after checking it with gogverify.
However, MD5 is weak against collisions, so the developer could theoretically construct two different versions of a game with the same MD5 hash, which this tool cannot detect.
For example, a developer might upload a modified copy to a piracy website.

It might also be possible to place malicious files inside the game folder without modifying any existing files, so make sure to check the "unexpected files".

[innoextract](https://constexpr.org/innoextract/) can be used to extract installers without executing them.

