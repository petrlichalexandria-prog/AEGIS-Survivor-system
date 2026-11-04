# AEGIS (Autonomous Evidentiary Grounding & Incident System)

> **Current Status:** Architectural Proposal & Concept Specification  
> **Repository Purpose:** System design, JSON data schema, and open-source proposal. *Not a compiled or audited production mobile app.*

AEGIS is an open-source, survivor-designed architectural framework for high-conflict incident logging and evidence organization across domestic, workplace, child protection, and institutional abuse environments[span_4](start_span)[span_4](end_span)[span_5](start_span)[span_5](end_span).

---

## 1. Project Overview & Scope

AEGIS bridges the gap between daily high-conflict situations and official legal/advocacy review. The goal of this architecture is to help self-represented individuals convert chaotic, emotionally charged experiences into structured, objective, time-stamped documentation.

* **What is defined in this repository:** Complete JSON system schema, incident categorization taxonomy, and behavioral extraction guidelines[span_6](start_span)[span_6](end_span)[span_7](start_span)[span_7](end_span).
* **What requires development & review:** Compiled mobile app software container (iOS/Android), OS-level hardware trigger integration, client-side encryption key management, and security/privacy audits[span_8](start_span)[span_8](end_span)[span_9](start_span)[span_9](end_span).

---

## 2. Architecture Blueprint & Data Schema

```json
{
  "AEGIS (Autonomous Evidentiary Grounding & Incident System)": {
    "version": "0.1.0",
    "type": "Open-Source Non-Profit Collaboration Proposal",
    "description": "Encrypted, offline-first survivor documentation platform and high-conflict incident logger specification.",
    "architecture_targets": {
      "frontend": "Progressive Web App (PWA) / Cross-Platform Mobile (React Native / Flutter)",
      "database": "Local-First Encrypted Database (SQLite / IndexedDB with AES-256-GCM)",
      "security_goals": "Planned Client-Side Encryption, Biometric Lock, PIN Decryption, Steganographic UX"
    },
    "proposed_modules": {
      "MOD-01": {
        "name": "Vault & Encrypted Database Specification",
        "features": [
          "Client-side encryption prior to disk write",
          "No forced cloud sync to mitigate remote subpoena or account compromise risks",
          "EXIF metadata preservation for media (timestamps, geolocation tags)",
          "Structured export formats intended for legal and advocate review (with SHA-256 integrity verification)"
        ]
      },
      "MOD-02": {
        "name": "Conflict Acoustic & Sensor Trigger Concept",
        "features": [
          "Audio level monitoring (dB threshold detection for elevated voices)",
          "Hardware shortcuts (volume button sequence, motion/shake activation)",
          "Auto-buffering short audio clips into local encrypted vault"
        ]
      },
      "MOD-03": {
        "name": "Discreet UX & Safety Safeguards",
        "features": [
          "Optional utility icon disguise (e.g., standard calculator or utility tool)",
          "Duress panic PIN concept (entering a designated PIN presents a clean workspace while keeping real data locked)"
        ]
      },
      "MOD-04": {
        "name": "Incident Cataloging & Categorization Schema",
        "categories": [
          "Aggression / Escalation",
          "Environmental / Safety Hazards",
          "Custody & Exchange Volatility",
          "Financial / Coercive Control",
          "Psychological Boundary Violations",
          "Co-parenting Communication Interference"
            ]
      },
      "MOD-05": {
        "name": "Trauma-Informed Sensory Memory Mapping",
        "features": [
          "Non-linear sensory prompting (lighting, weather, ambient sounds, clothing anchors)",
          "External contextual anchor-linking (cross-referencing calendar/weather history to establish precise timestamps)",
          "Spatial zone categorization for incident location framing"
        ]
      },
      "MOD-06": {
        "name": "Nervous System Pacing & Grounding Guardrails",
        "features": [
          "Real-time stress pattern detection (frantic typing speed, high emotional density)",
          "Automatic silent draft-saving with gentle pause prompts",
          "Micro-grounding physical resets (sip of cold water, shoulder drop, jaw unclench, 30-second sensory focal shift)"
        ]
      }
    },
      }
    },
    "incident_entry_schema": {
      "incident_id": "UUID v4",
      "timestamp": "ISO-8601",
      "severity_level": "LOW | MEDIUM | HIGH ALERT RED FLAG",
      "category_tag": "STRING",
      "observed_behaviors": ["STRING"],
      "factual_summary": {
        "objective_events": "STRING",
        "direct_quotes_or_text": "STRING",
        "impact_on_minors": "STRING",
        "third_party_reporting": "THERAPIST | SCHOOL COUNSELOR | PEDIATRICIAN | LEGAL | NONE"
      },
      "attached_media_refs": ["STRING"],
      "media_metadata": {
        "file_type": "AUDIO | IMAGE | DOCUMENT",
        "hash_sha256": "STRING",
        "exif_provenance": "STRING"
      },
      "third_party_notifications": [
        {
          "recipient_type": "THERAPIST | COUNSELOR | PEDIATRICIAN | LEGAL",
          "notification_id": "ISO-8601",
          "confirmation_status": "BOOLEAN"
        }
      ]
    }
  }
}
