# Runtime policy

```yaml workflow-v1
{
  "anti_gaming_rules": [
    {
      "ref": "gitpath:YW50aS1nYW1pbmcudHh0",
      "sha256": "48df105e8742f813b227f93954fc2f7f87cf5254d98e18c52cd8024a58b6f6ce"
    }
  ],
  "brief_template": {
    "ref": "artifact:fixture-brief",
    "sha256": "aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa"
  },
  "checks": [
    {
      "arguments": [
        "--candidate",
        "{candidate}",
        "--configuration",
        "{configuration:0}",
        "--selection",
        "{selection}",
        "--thresholds",
        "{thresholds}",
        "--tests",
        "{reference-test:0}",
        "--dependency",
        "{dependency:0}",
        "--output",
        "{output}",
        "--probe-input-writes"
      ],
      "base_sha": "0000000000000000000000000000000000000000",
      "check_id": "reference-contract",
      "command": "reference-verifier",
      "configuration": [
        {
          "ref": "gitpath:Y29uZmlndXJhdGlvbi50eHQ",
          "sha256": "3177f0925b2f166b1cd6f90aded36b5a8c91a9c918370af2e2f6c0d51a82b115"
        }
      ],
      "environment": {
        "dependency_sources": [],
        "environment_ref": {
          "ref": "environment:kh-e1-static-v1",
          "sha256": "41800c7ec05440c6e1b4195b740fdd6706146ae6fdba0964868b31d74512c4b5"
        },
        "input_paths": [
          "candidate",
          "reference"
        ],
        "output_paths": [
          "output"
        ],
        "permitted_variables": [],
        "resolution": "trusted-reference-only",
        "working_directory": "output"
      },
      "policy_source": {
        "ref": "gitpath:UE9MSUNZLmpzb24",
        "sha256": "5e66d8fc615a870d3c35228dc4ed5923a9d7e37be6e2e53ddb2b112e60210b02"
      },
      "reference_tests": [
        {
          "ref": "gitpath:cmVmZXJlbmNlLXRlc3RzLnR4dA",
          "sha256": "8c82ffc0f7cf9306681ab7ef55a52995a31a13a1e09c00117eca4bc3bacdfcd5"
        }
      ],
      "selection": {
        "ref": "gitpath:c2VsZWN0aW9uLnR4dA",
        "sha256": "525e597535b63b981f6911a9bd7864c1af43b9b60f813cf63e8f8c455bce0ad5"
      },
      "thresholds": {
        "ref": "gitpath:dGhyZXNob2xkcy50eHQ",
        "sha256": "ba32b1cfdbcc62fc7b70387bea319774c3c0153637dd390920e4ed28f121ca0f"
      },
      "transitive_dependencies": [
        {
          "authority": "trusted",
          "ref": {
            "ref": "gitpath:ZGVwZW5kZW5jeS50eHQ",
            "sha256": "6b069acc842db77c35204fe51103d201bceb9b06103ee40dc42bd9a68ee29387"
          },
          "version": "1"
        }
      ],
      "verifier_code": [
        {
          "ref": "gitpath:cmVmZXJlbmNlLWNoZWNr",
          "sha256": "0a7e3085b219819440d931d097f4603b625124e73b8f2a295dff8d087255d621"
        }
      ]
    }
  ],
  "defaults": {
    "review_mode": "agent",
    "token_budget": 50000
  },
  "network_profile": {
    "authority": "trusted",
    "ref": {
      "ref": "artifact:deny-default",
      "sha256": "dddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddd"
    },
    "version": "1"
  },
  "required_egress": [],
  "runtime": {
    "provider_profile": {
      "authority": "trusted",
      "ref": {
        "ref": "artifact:codex-subscription",
        "sha256": "cccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccc"
      },
      "version": "1"
    },
    "sandbox_profile": {
      "authority": "trusted",
      "ref": {
        "ref": "artifact:d1-kh-native-v2",
        "sha256": "bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb"
      },
      "version": "2"
    },
    "stall_seconds": 120,
    "turn_silence_seconds": 60
  },
  "schema_version": 1,
  "sensitive_paths": [
    "secrets"
  ],
  "services": []
}
```
