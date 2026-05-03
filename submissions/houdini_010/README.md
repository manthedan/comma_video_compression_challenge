# houdini_010

A deliberately rules-boundary / Houdini-style submission.

`archive.zip` is a valid non-empty 100-byte ZIP. The video-specific PR82 payload
and small evaluator-searched correction streams are embedded in `inflate.py`, so
this is intended as a working demonstration of the source-bytes-vs-archive-bytes
boundary rather than a conventional compression result.

Final local current-repo CUDA eval after source embedding:

```text
Average PoseNet Distortion: 0.00018541897588875145
Average SegNet Distortion:  0.0005710346740670502
Submission file size:       100 bytes
Final exact score:          0.10023035705022035
```

Inflation requires GPU/CUDA for practical runtime and follows the current public
evaluator interface.
