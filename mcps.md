# Installed MCP Servers & Tools

This document lists all installed Model Context Protocol (MCP) servers and their available tools.

## Overview

| Server Name | Tools Count |
| --- | --- |
| [astronomer](#astronomer) | 51 |
| [biologist](#biologist) | 51 |
| [blender](#blender) | 10 |
| [book-rhino](#book-rhino) | 74 |
| [chemist](#chemist) | 51 |
| [devbook](#devbook) | 17 |
| [evox](#evox) | 10 |
| [godot](#godot) | 14 |
| [macron-cms](#macron-cms) | 12 |
| [macronx](#macronx) | 7 |
| [mcp-motion](#mcp-motion) | 30 |
| [memorable](#memorable) | 17 |
| [noteking](#noteking) | 18 |
| [physicist](#physicist) | 51 |
| [statesman](#statesman) | 51 |
| [syncretica](#syncretica) | 46 |
| [wikidata](#wikidata) | 7 |

---

## astronomer

**Total Tools:** 51

- **`compute_clusters`** - Compute live connected-components vector clusters for StarSystems or CelestialBodies across cosmic structures without modifying the database.
- **`create_celestial_body`** - Create a new celestial body record associated with a star system.
- **`create_cluster_report`** - Initiate a 2-Phase Map-Reduce synthesis report on a frozen cluster snapshot.
- **`create_cluster_snapshot`** - Compute connected-components clustering and freeze it immediately into an immutable database snapshot.
- **`create_cosmic_structure`** - Create a new cosmic structure (galaxy or cluster) record in the catalog.
- **`create_star_system`** - Create a new star system record associated with a cosmic structure.
- **`delete_celestial_body`** - Delete a celestial body record.
- **`delete_cluster_report`** - Delete a synthesis report along with its intermediate summaries and sub-reports.
- **`delete_cluster_snapshot`** - Delete a frozen cluster snapshot along with its cascaded cluster groups and synthesis reports.
- **`delete_cosmic_structure`** - Delete a cosmic structure and its cascaded star systems and celestial bodies.
- **`delete_star_system`** - Delete a star system and its cascaded celestial bodies.
- **`find_counterparts`** - Find nearest astrophysical counterparts to a specified star system or celestial body using 1024-dimensional pgvector cosine distance.
- **`generate_celestial_body_embedding`** - Calculate 1024-dimensional vector embedding for a celestial body record.
- **`generate_deep_synthesis`** - Initiate a 3-Phase Hierarchical Deep Synthesis monograph, reusing Phase 1 summaries from a completed parent report.
- **`generate_star_system_embedding`** - Calculate 1024-dimensional vector embedding for a star system using the configured embedding model.
- **`get_celestial_body`** - Retrieve details of a celestial body including its structured themes and associated star system/cosmic structure.
- **`get_cluster_group`** - Retrieve details of a specific archetype cluster group with all member star systems or celestial bodies.
- **`get_cluster_report`** - Retrieve complete scholarly astrophysics report content, progress percentage, markdown monograph, and intermediate summaries.
- **`get_cluster_snapshot`** - Retrieve details of a frozen cluster snapshot including member groups and generated reports.
- **`get_cosmic_structure`** - Retrieve details of a single cosmic structure (galaxy/cluster) including its star systems.
- **`get_job_status`** - Check the status, progress, and result of an ActiveJob/Sidekiq background task.
- **`get_openapi_spec`** - Retrieve the raw OpenAPI 3.1 specification for the Astronomer API.
- **`get_platform_status`** - Get overall platform health, catalog entity counts, embedding coverage stats, and active LLM configuration.
- **`get_report_sub_report`** - Retrieve a single Phase 2 batch analysis.
- **`get_report_summary`** - Retrieve a single Phase 1 per-cluster scholarly summary.
- **`get_settings`** - Get embedding completion metrics for StarSystems and CelestialBodies, active embedding/LLM parameters, and context window presets.
- **`get_star_system`** - Retrieve full profile of a star system including cosmic structure, thematic astrophysical tags, and celestial bodies.
- **`list_celestial_bodies`** - List and filter celestial bodies (exoplanets, moons, dwarf planets) with physical/orbital themes and embedding metadata.
- **`list_cluster_groups`** - List all archetype cluster groups belonging to a specific frozen snapshot.
- **`list_cluster_reports`** - List generated multi-phase comparative astrophysics and celestial body manifold synthesis reports.
- **`list_cluster_snapshots`** - List frozen archetype cluster snapshots.
- **`list_cosmic_structures`** - List cosmic structures (galaxies, dwarf galaxies, galaxy clusters) registered in Astronomer with star system counts.
- **`list_jobs`** - List recent asynchronous background jobs (embedding calculations, LLM discoveries, synthesis reports).
- **`list_report_sub_reports`** - List all Phase 2 intermediate batch analyses belonging to a detailed synthesis report.
- **`list_report_summaries`** - List all Phase 1 per-cluster analyses belonging to a synthesis report.
- **`list_star_systems`** - List and filter star systems with astrophysical themes, celestial body counts, and vector embedding status.
- **`populate_celestial_bodies_bulk`** - Trigger bulk LLM celestial body discovery across all star systems or a single star system.
- **`populate_cosmic_structure_star_systems`** - Discover and populate star systems for a specific cosmic structure via LLM generation.
- **`populate_cosmic_structures`** - Trigger LLM discovery to populate major galaxies and galaxy clusters with astrophysical descriptions.
- **`populate_star_system_celestial_bodies`** - Discover and generate celestial bodies (planets, moons) for a star system via LLM extraction.
- **`populate_star_systems_bulk`** - Trigger bulk LLM star system discovery across all cosmic structures or a single cosmic structure.
- **`search`** - Unified cross-catalog semantic or keyword search across star systems and celestial bodies in the Astronomer comparative astrophysics manifold.
- **`trigger_bulk_embeddings`** - Enqueue bulk embedding generation for all StarSystems or CelestialBodies.
- **`update_celestial_body`** - Update an existing celestial body's attributes, star system, or thematic tags.
- **`update_context_window`** - Dynamically update the active LLM context window token size.
- **`update_cosmic_structure`** - Update an existing cosmic structure's name or description.
- **`update_star_system`** - Update an existing star system's attributes, cosmic structure, or thematic tags.
- **`upsert_celestial_bodies_batch`** - Batch insert or update celestial bodies scoped to a specific star system.
- **`upsert_cosmic_structures_batch`** - Batch insert or update cosmic structures matching case-insensitively on name.
- **`upsert_star_systems_batch`** - Batch insert or update star systems scoped to a specific cosmic structure.
- **`wait_for_job`** - Poll a background job until completion or failure with configurable timeout.

---

## biologist

**Total Tools:** 51

- **`compute_clusters`** - Compute live connected-components vector clusters for Species or Organisms across biomes without modifying the database.
- **`create_biome`** - Create a new biome record in the catalog.
- **`create_cluster_report`** - Initiate a 2-Phase Map-Reduce synthesis report on a frozen cluster snapshot.
- **`create_cluster_snapshot`** - Compute connected-components clustering and freeze it immediately into an immutable database snapshot.
- **`create_organism`** - Create a new individual organism/morph record under a parent species.
- **`create_species`** - Create a new species record under a parent biome.
- **`delete_biome`** - Delete a biome and its cascaded species and organisms.
- **`delete_cluster_report`** - Delete a synthesis report along with its intermediate summaries and sub-reports.
- **`delete_cluster_snapshot`** - Delete a frozen cluster snapshot along with its cascaded cluster groups and synthesis reports.
- **`delete_organism`** - Delete an individual organism record.
- **`delete_species`** - Delete a species and its associated individual organisms.
- **`find_counterparts`** - Find nearest ecological counterparts or convergent evolutionary analogs to a specified species or organism using 1024-dimensional pgvector cosine distance.
- **`generate_deep_synthesis`** - Initiate a 3-Phase Hierarchical Deep Synthesis monograph, reusing Phase 1 summaries from a completed parent report.
- **`generate_organism_embedding`** - Generate or refresh the 1024-dimensional semantic embedding for an individual organism.
- **`generate_species_embedding`** - Generate or refresh the 1024-dimensional semantic embedding for a species.
- **`get_biome`** - Retrieve details of a single biome including its member species.
- **`get_cluster_group`** - Retrieve details of a specific archetype cluster group with all member species or organisms.
- **`get_cluster_report`** - Retrieve complete scholarly biological report content, progress percentage, markdown monograph, and intermediate summaries.
- **`get_cluster_snapshot`** - Retrieve details of a frozen cluster snapshot including member groups and generated synthesis reports.
- **`get_job_status`** - Check the status, progress, and result of an ActiveJob/Sidekiq background task.
- **`get_openapi_spec`** - Retrieve the raw OpenAPI 3.1 specification for the Biologist API.
- **`get_organism`** - Retrieve details of a single individual organism including parent species and biome.
- **`get_platform_status`** - Get overall platform health, catalog entity counts, embedding coverage stats, and active LLM configuration.
- **`get_report_sub_report`** - Retrieve a single Phase 2 batch analysis.
- **`get_report_summary`** - Retrieve a single Phase 1 per-cluster scholarly summary.
- **`get_settings`** - Get embedding completion metrics for Species and Organisms, active embedding/LLM parameters, and context window presets.
- **`get_species`** - Retrieve details of a single biological species including its biome and child organisms.
- **`list_biomes`** - List biomes (global ecosystems, climatic zones, and primary environmental regimes) registered in Biologist with species counts.
- **`list_cluster_groups`** - List all archetype cluster groups belonging to a specific frozen snapshot.
- **`list_cluster_reports`** - List generated multi-phase comparative biology and ecological manifold synthesis reports.
- **`list_cluster_snapshots`** - List frozen archetype cluster snapshots in Biologist.
- **`list_jobs`** - List recent asynchronous background jobs (embedding calculations, LLM discoveries, synthesis reports).
- **`list_organisms`** - List individual organisms (morphs, castes, sexual dimorphisms, life-history stages) with filtering by species, biome, themes, and embedding status.
- **`list_report_sub_reports`** - List all Phase 2 intermediate batch analyses belonging to a detailed synthesis report.
- **`list_report_summaries`** - List all Phase 1 per-cluster analyses belonging to a synthesis report.
- **`list_species`** - List species registered in Biologist with filtering by biome, themes, embedding status, and search keywords.
- **`populate_biome_species`** - Discover and populate canonical species for a specific biome via LLM generation.
- **`populate_biomes`** - Trigger LLM discovery to populate major global biomes and environmental regimes.
- **`populate_organisms_bulk`** - Trigger LLM discovery to populate individual organisms across all registered species.
- **`populate_species_bulk`** - Trigger LLM discovery to populate species across all registered biomes.
- **`populate_species_organisms`** - Discover and populate individual organisms, castes, or morphs for a specific species via LLM generation.
- **`search`** - Unified cross-catalog semantic or keyword search across species and individual organisms in the Biologist comparative biology manifold.
- **`trigger_bulk_embeddings`** - Enqueue bulk embedding generation for all Species or Organisms.
- **`update_biome`** - Update an existing biome's name or description.
- **`update_context_window`** - Dynamically update the active LLM context window token size.
- **`update_organism`** - Update an existing organism's attributes, species assignment, or themes.
- **`update_species`** - Update an existing species's attributes, biome assignment, or themes.
- **`upsert_biomes_batch`** - Batch insert or update biomes matching case-insensitively on name.
- **`upsert_organisms_batch`** - Batch insert or update organisms scoped to a specific species matching case-insensitively on name.
- **`upsert_species_batch`** - Batch insert or update species scoped to a specific biome matching case-insensitively on name.
- **`wait_for_job`** - Poll a background job until completion or failure with configurable timeout.

---

## blender

**Total Tools:** 10

- **`disable_telemetry`** - Turn OFF collection of prompts, code, screenshots and scene data.
- **`execute_blender_code`** - Run Python in the user's live Blender (bpy, bmesh, mathutils). Whatever it prints is returned.
- **`generate_3d`** - Make one new textured 3D model from a text prompt or an image, and import it.
- **`generate_gaussian_world`** - Generate a whole environment with World Labs Marble and import it as Gaussian splats (a photoreal capture of the place, not editable meshes), with a hidden rough collision mesh for placing objects and its panorama as the world background, in metres with the ground at z=0. Needs Blender 5.3+.
- **`get_addon_status`** - Check the connected Blender: its version, whether the addon matches this server, and which asset libraries and 3D generators are switched on. Call it once at the start.
- **`get_scene_info`** - Facts about the scene as text: what's there, where, how big, and how healthy meshes and rigs are. No image; to see the scene, use look.
- **`import_asset`** - Download an asset found with search_assets and bring it into the scene.
- **`look`** - See the scene as one image. For counts, sizes and positions, use get_scene_info.
- **`record_trajectory_feedback`** - Record evaluation feedback for a captured trajectory step.
- **`search_assets`** - Search a library of existing assets. The sources: - polyhaven: HDRIs, PBR textures and realistic models, all CC0. Search understands intent and synonyms ("couch" finds sofas). - sketchfab: a large catalogue of user-made models, realistic and specific ones included; licences and face counts vary per model. - polypizza: stylised low-poly models, CC0 or CC-BY (credit the creator).

---

## book-rhino

**Total Tools:** 74

- **`attach_image`** - Upload and attach a portrait or concept image to a character or location. Provide exactly one source: local file_path (<= 25MB), remote public image_url, or image_base64.
- **`check_health`** - Check connectivity and health status of the Book Rhino REST API v1.
- **`create_book`** - Create a new book. Requires title, writing_style_id, perspective_id, and narrative_structure_id. Note: protagonist_id, antagonist_ids, and supporting character_ids must be mutually exclusive.
- **`create_chapter`** - Create a new chapter for a book. Requires book_id, unique positive chapter number, name, and outline.
- **`create_character`** - Create a new character profile with biographical attributes and taxonomy associations (character_types, moral_alignments, personality_traits, archetypes, locations).
- **`create_location`** - Create a new location with atmospheric/sensory attributes. Both name (unique) and description are required.
- **`create_region`** - Create a new geographic or worldbuilding region to group locations.
- **`create_scene`** - Create a new scene inside a chapter.
- **`create_taxonomy_item`** - Create a new record in one of the 8 taxonomy collections. Allowed attributes by taxonomy: perspectives: { name, narrator?, pronouns?, effect?, example? }; archetypes: { name, traits?, examples? }; personality_traits: { name, description? }; moral_alignments: { name (required), description (required), examples?: string[] }; narrative_structures: { name (required), description?, parts?: Record<string, unknown> }; character_types: { name, definition?, purpose?, example? }; poetic_forms: { name (required), description?, meter?, rhyme_scheme?, guidelines?, example? }; cinematic_styles: { name (required), aesthetic_tags (required), description?, lighting?, example? }.
- **`create_text`** - Attach a sample prose excerpt/corpus text to a writing style for style analysis.
- **`create_writing_style`** - Create a new writing style. You can attach sample prose excerpts via create_text and then synthesize the style prompt via generate_writing_style_prompt, or provide a JSON prompt object directly.
- **`delete_book`** - Permanently delete a book and all of its dependent chapters and scenes.
- **`delete_chapter`** - Delete a chapter and all of its scenes.
- **`delete_character`** - Delete a character and their attached portrait images.
- **`delete_image`** - Delete an attached character or location image.
- **`delete_location`** - Delete a location and its attached reference images.
- **`delete_region`** - Delete a region by ID.
- **`delete_scene`** - Delete a scene by ID.
- **`delete_taxonomy_item`** - Delete a taxonomy item by collection type and ID.
- **`delete_text`** - Delete a reference sample text by ID.
- **`delete_writing_style`** - Delete a writing style and its attached sample texts.
- **`generate_book_plot`** - Enqueue AI plot and chapter-outline generation for a book (GenerateBookPlotJob). Tip: generate AI prompts on linked characters and locations first so their prompts are woven into the plot.
- **`generate_chapter_scenes`** - Break a rendered chapter down into structured scenes via AI (WriteScenesJob). Prerequisite: chapter must have rendered content AND scene_count > 0 (use update_chapter to set scene_count first if needed).
- **`generate_character_prompt`** - Synthesize a rich AI narrative prompt from the character's attributes and taxonomy tags (GenerateCharacterPromptJob).
- **`generate_location_prompt`** - Synthesize an atmospheric AI worldbuilding prompt for a location (GenerateLocationPromptJob).
- **`generate_writing_style_prompt`** - Analyze the writing style's attached sample texts and synthesize a structured JSON style prompt via AI (GenerateWritingStyleJob).
- **`get_book`** - Retrieve full details of a book including its taxonomies, protagonist, antagonists, supporting characters, locations, and ordered chapters/scenes.
- **`get_book_manuscript`** - Export or read the compiled Markdown manuscript for a book. Supports saving directly to a local file via output_path (returning word counts and a chapter table of contents without flooding context) and omits duplicate chapter JSON prose by default.
- **`get_chapter`** - Retrieve a single chapter by ID, including its outline, prose content, summary, word count, can_render status, and scenes.
- **`get_character`** - Retrieve full character sheet including biography, psychology, synthesized AI prompt, taxonomy tags, linked locations, and portrait images.
- **`get_image`** - Retrieve metadata and resolved download URL for a single character or location image.
- **`get_location`** - Retrieve full location details including sensory attributes, region, AI prompt, linked character IDs, and reference images.
- **`get_me`** - Retrieve the authenticated Book Rhino user profile, access status, and admin role.
- **`get_operation`** - Inspect the current status, timestamps, metadata, and error details of a single Sidekiq operation.
- **`get_region`** - Retrieve a single region by ID.
- **`get_scene`** - Retrieve a single scene by ID including its outline, rendered content, and summary.
- **`get_settings`** - Retrieve global Book Rhino platform settings, LLM prompt templates, model tunings, and publish window status.
- **`get_taxonomy_item`** - Retrieve a single taxonomy item by collection type and ID.
- **`get_text`** - Retrieve a single reference prose corpus text by ID.
- **`get_writing_style`** - Retrieve a single writing style by ID, optionally including its attached prose corpus sample texts.
- **`iterate_book_plot`** - Refine an existing book plot and chapter outlines via AI feedback instructions (IterateOnBookPlotJob).
- **`iterate_character_prompt`** - Refine an existing character prompt via natural-language feedback instructions (IterateOnCharacterPromptJob).
- **`iterate_location_prompt`** - Refine a location's AI prompt with natural-language instructions (IterateOnLocationPromptJob).
- **`iterate_writing_style_prompt`** - Refine a writing style's JSON prompt via AI instructions (IterateOnWritingStyleJob).
- **`list_all_taxonomies`** - Fetch all 8 creative taxonomy dictionaries (perspectives, archetypes, personality_traits, moral_alignments, narrative_structures, character_types, poetic_forms, cinematic_styles) plus writing_styles in one parallel snapshot. Call this before creating books or characters to resolve valid IDs.
- **`list_books`** - List and search books in Book Rhino with filters for writing style, perspective, narrative structure, and AI pending/rendering state.
- **`list_chapters`** - List chapters ordered by chapter number, typically filtered by book_id.
- **`list_characters`** - List and search characters alphabetically, optionally filtered by name query or book_id.
- **`list_images`** - List attached images for a character or location with resolved ActiveStorage blob URLs.
- **`list_locations`** - List and search worldbuilding locations, optionally filtered by query, region_id, or book_id.
- **`list_operations`** - List asynchronous Sidekiq AI generation and rendering operations with optional status and resource filters.
- **`list_regions`** - List geographic or worldbuilding regions with optional search query or country filter.
- **`list_scenes`** - List scenes ordered by scene number, filtered by chapter_id or book_id.
- **`list_taxonomy_items`** - List or search records within one of Book Rhino's 8 creative taxonomy collections.
- **`list_texts`** - List reference prose corpus texts used to train/analyze writing styles.
- **`list_versions`** - List PaperTrail version history and field diffs for a versioned resource (books, characters, locations, or writing_styles).
- **`list_writing_styles`** - List writing styles with their parsed JSON style prompts and attached sample text counts.
- **`merge_version`** - Synthesize and merge changes from a historical PaperTrail version into the current prompt/plot using AI (MergeBookPlotsJob / MergeCharacterPromptsJob / MergeLocationPromptsJob / MergeWritingStylesJob).
- **`render_book`** - Enqueue full-book prose rendering across all chapters sequentially (RenderBookJob). Defaults to wait=false because rendering an entire book can take several minutes; monitor via wait_for_operation or get_operation.
- **`render_chapter`** - Render full prose content and summary for a chapter using AI (RenderChapterJob). Prerequisite: previous chapters in the book must already be rendered (can_render=true).
- **`render_scene`** - Render detailed visual/prose content for a scene via AI (RenderSceneJob), with optional cinematic shot_type and style overrides.
- **`revert_version`** - Revert a book, character, location, or writing_style back to the state captured in a specific PaperTrail version (note: initial creation versions cannot be reified).
- **`update_book`** - Update an existing book's metadata, plot, taxonomy links, cast roles, or locations. Protagonist, antagonist, and supporting character IDs must remain mutually exclusive.
- **`update_chapter`** - Update a chapter's number, name, outline, prose content, summary, or target scene_count.
- **`update_character`** - Update an existing character's attributes, prompt, or taxonomy associations.
- **`update_image`** - Update the display title of an attached character or location image.
- **`update_location`** - Update an existing location's sensory attributes, region, prompt, or associated characters.
- **`update_region`** - Update an existing region's name, city, state, country, or description.
- **`update_scene`** - Update a scene's number, outline, content, or summary.
- **`update_settings`** - Update global Book Rhino LLM prompts, tunings, image prompts, or publish window (requires admin user AND BOOK_RHINO_ALLOW_ADMIN=true).
- **`update_taxonomy_item`** - Update an existing taxonomy record. Allowed attributes by taxonomy: perspectives: { name, narrator?, pronouns?, effect?, example? }; archetypes: { name, traits?, examples? }; personality_traits: { name, description? }; moral_alignments: { name (required), description (required), examples?: string[] }; narrative_structures: { name (required), description?, parts?: Record<string, unknown> }; character_types: { name, definition?, purpose?, example? }; poetic_forms: { name (required), description?, meter?, rhyme_scheme?, guidelines?, example? }; cinematic_styles: { name (required), aesthetic_tags (required), description?, lighting?, example? }.
- **`update_text`** - Update a reference sample text's name or prose corpus.
- **`update_writing_style`** - Update an existing writing style's name or JSON prompt.
- **`wait_for_operation`** - Poll an asynchronous Sidekiq operation until it succeeds, fails, or reaches timeout_ms, automatically returning the refreshed target resource.

---

## chemist

**Total Tools:** 51

- **`compute_clusters`** - Compute live connected-components vector clusters for Molecules or FunctionalGroups across chemical classes without modifying the database.
- **`create_chemical_class`** - Create a new chemical class record in the catalog.
- **`create_cluster_report`** - Initiate a 2-Phase Map-Reduce synthesis report on a frozen cluster snapshot.
- **`create_cluster_snapshot`** - Compute connected-components clustering and freeze it immediately into an immutable database snapshot.
- **`create_functional_group`** - Create a new functional group or reactive motif under a molecule.
- **`create_molecule`** - Create a new molecule record in Chemist.
- **`delete_chemical_class`** - Delete a chemical class and its cascaded molecules and functional groups.
- **`delete_cluster_report`** - Delete a synthesis report along with its intermediate summaries and sub-reports.
- **`delete_cluster_snapshot`** - Delete a frozen cluster snapshot along with its cascaded cluster groups and synthesis reports.
- **`delete_functional_group`** - Delete a functional group from the catalog.
- **`delete_molecule`** - Delete a molecule and its cascaded functional groups.
- **`find_counterparts`** - Find nearest chemical counterparts or bioisosteric analogs to a specified molecule or functional group using 1024-dimensional pgvector cosine distance.
- **`generate_deep_synthesis`** - Initiate a 3-Phase Hierarchical Deep Synthesis monograph, reusing Phase 1 summaries from a completed parent report.
- **`generate_functional_group_embedding`** - Generate or regenerate a 1024-dimensional semantic embedding vector for a functional group.
- **`generate_molecule_embedding`** - Generate or regenerate a 1024-dimensional semantic embedding vector for a single molecule.
- **`get_chemical_class`** - Retrieve details of a single chemical class including its molecules.
- **`get_cluster_group`** - Retrieve details of a specific archetype cluster group with all member molecules or functional groups.
- **`get_cluster_report`** - Retrieve complete scholarly chemistry report content, progress percentage, markdown monograph, and intermediate summaries.
- **`get_cluster_snapshot`** - Retrieve details of a frozen cluster snapshot including member groups and generated synthesis reports.
- **`get_functional_group`** - Retrieve details of a single functional group including parent molecule and chemical class metadata.
- **`get_job_status`** - Check the status, progress, and result of an ActiveJob/Sidekiq background task.
- **`get_molecule`** - Retrieve details of a single molecule including its chemical class and child functional groups.
- **`get_openapi_spec`** - Retrieve the raw OpenAPI 3.1 specification for the Chemist API.
- **`get_platform_status`** - Get overall platform health, catalog entity counts, embedding coverage stats, and active LLM configuration.
- **`get_report_sub_report`** - Retrieve a single Phase 2 batch analysis.
- **`get_report_summary`** - Retrieve a single Phase 1 per-cluster scholarly summary.
- **`get_settings`** - Get embedding completion metrics for Molecules and FunctionalGroups, active embedding/LLM parameters, and context window presets.
- **`list_chemical_classes`** - List chemical classes (superfamilies, biosynthetic families, compound classes) registered in Chemist with molecule counts.
- **`list_cluster_groups`** - List all archetype cluster groups belonging to a specific frozen snapshot.
- **`list_cluster_reports`** - List generated multi-phase comparative chemistry and molecular manifold synthesis reports.
- **`list_cluster_snapshots`** - List frozen archetype cluster snapshots in Chemist.
- **`list_functional_groups`** - List functional groups and reactive motifs registered in Chemist with filtering by molecule, chemical class, themes, and embedding status.
- **`list_jobs`** - List recent asynchronous background jobs (embedding calculations, LLM discoveries, synthesis reports).
- **`list_molecules`** - List molecules registered in Chemist with filtering by chemical class, themes, embedding status, and search keywords.
- **`list_report_sub_reports`** - List all Phase 2 intermediate batch analyses belonging to a detailed synthesis report.
- **`list_report_summaries`** - List all Phase 1 per-cluster analyses belonging to a synthesis report.
- **`populate_chemical_class_molecules`** - Discover and populate molecules for a specific chemical class via LLM generation.
- **`populate_chemical_classes`** - Trigger LLM discovery to populate major chemical classes and superfamilies with biochemical descriptions.
- **`populate_functional_groups_bulk`** - Bulk trigger discovery of functional groups across all molecules under an optional molecule scope.
- **`populate_molecule_functional_groups`** - Discover and populate functional groups and reactive motifs for a molecule via LLM analysis.
- **`populate_molecules_bulk`** - Bulk trigger discovery of molecules across one or all chemical classes via background job.
- **`search`** - Unified cross-catalog semantic or keyword search across molecules and functional groups in the Chemist comparative chemistry manifold.
- **`trigger_bulk_embeddings`** - Enqueue bulk embedding generation for all Molecules or FunctionalGroups.
- **`update_chemical_class`** - Update an existing chemical class's name or description.
- **`update_context_window`** - Dynamically update the active LLM context window token size.
- **`update_functional_group`** - Update an existing functional group's attributes.
- **`update_molecule`** - Update an existing molecule's attributes (name, description, themes, or parent chemical class).
- **`upsert_chemical_classes_batch`** - Batch insert or update chemical classes matching case-insensitively on name.
- **`upsert_functional_groups_batch`** - Batch insert or update functional groups for a specific molecule matching on lower(name).
- **`upsert_molecules_batch`** - Batch insert or update molecules under a specific chemical class matching on lower(name).
- **`wait_for_job`** - Poll a background job until completion or failure with configurable timeout.

---

## devbook

**Total Tools:** 17

- **`devbook_create_project`** - Create a new prompt project workspace in Devbook
- **`devbook_create_prompt`** - Create a new prompt template in Devbook (under a project or as a standalone scratchpad prompt)
- **`devbook_delete_attachment`** - Purge and delete an attachment from a prompt
- **`devbook_delete_project`** - Delete a project from Devbook (prompts in the project become standalone or are deleted depending on cascade)
- **`devbook_delete_prompt`** - Permanently delete a prompt and its attachments from Devbook
- **`devbook_get_project`** - Get full project details including its prompt list index and metadata
- **`devbook_get_prompt`** - Retrieve a prompt's full Markdown template content, metadata, attachments, and optional rendered HTML
- **`devbook_get_stats`** - Get system statistics from Devbook (total prompts, projects, attachments, pinned prompts, standalone prompts)
- **`devbook_list_attachments`** - List file attachments associated with a prompt
- **`devbook_list_projects`** - List and search prompt projects / workspaces in Devbook with prompt count metrics and pagination
- **`devbook_list_prompts`** - List, filter, and search prompts in Devbook by full-text search, project, standalone scope, or pinned status
- **`devbook_render_markdown`** - Render Markdown text to sanitized HTML using Devbook's GitHub-flavored markdown pipeline
- **`devbook_reorder_pinned`** - Update the sequential order of pinned prompts displayed in the Devbook sidebar
- **`devbook_toggle_pin`** - Toggle the pinned status of a prompt on the Devbook sidebar
- **`devbook_update_project`** - Update an existing project's name or description
- **`devbook_update_prompt`** - Update a prompt template's title, Markdown body, project assignment, or pinned status
- **`devbook_upload_attachment`** - Upload one or more files to attach to a prompt in Devbook (accepts local file paths or base64 data)

---

## evox

**Total Tools:** 10

- **`create_song`** - Creates a new song from a validated structured AST. Automatically formats and serializes to .evox markup.
- **`delete_song`** - Deletes a song (.evox file) from the songs/ folder.
- **`generate_songbook`** - Compiles the songbook into book/book.pdf using 'evox generate'. Automatically cleans stray OS files from songs/, validates all song syntax, and returns the generated PDF details with the alphabetical Table of Contents.
- **`get_cover`** - Reads cover/config.yml configuration (header, logo dimensions, footer) and logo image file status.
- **`get_song`** - Retrieves the full structured AST for a song by slug (including title, artist, font, column width, gutter, and all column/stanza lines with chord-lyric pairs).
- **`get_songbook`** - Returns comprehensive status of the songbook: directory initialization, cover settings, logo presence, song summaries in alphabetical print order, stray file warnings, and PDF build freshness.
- **`init_songbook`** - Initializes a new Evox songbook project directory structure (book/, cover/, songs/) using 'evox init'.
- **`list_songs`** - Lists all songs in the songbook in alphabetical print order (matching the order in the compiled PDF and Table of Contents).
- **`update_cover`** - Updates cover/config.yml settings (header titles/padding, logo size/image name, footer title/size) and optionally copies a new local image into cover/.
- **`update_song`** - Updates an existing song. Supports partial metadata changes, replacing columns, and/or renaming the song slug.

---

## godot

**Total Tools:** 14

- **`add_node`** - Add a node to an existing scene
- **`create_scene`** - Create a new Godot scene file
- **`export_mesh_library`** - Export a scene as a MeshLibrary resource
- **`get_debug_output`** - Get the current debug output and errors
- **`get_godot_version`** - Get the installed Godot version
- **`get_project_info`** - Retrieve metadata about a Godot project
- **`get_uid`** - Get the UID for a specific file in a Godot project (for Godot 4.4+)
- **`launch_editor`** - Launch Godot editor for a specific project
- **`list_projects`** - List Godot projects in a directory
- **`load_sprite`** - Load a sprite into a Sprite2D node
- **`run_project`** - Run the Godot project and capture output
- **`save_scene`** - Save changes to a scene file
- **`stop_project`** - Stop the currently running Godot project
- **`update_project_uids`** - Update UID references in a Godot project by resaving resources (for Godot 4.4+)

---

## macron-cms

**Total Tools:** 12

- **`add_content_block`** - Insert a single content block into an article at a specific position (or append to the end). Automatically shifts existing blocks down and normalizes sequence order.
- **`convert_content_block`** - Convert a content block in-place to a compatible target type (e.g. image <-> three_js_image) defined by the schema's `convertible_to` rules. Preserves existing file attachments and dormant JSON payload keys.
- **`create_article`** - Create a new article (or upsert an existing article) with metadata and ordered content blocks in a single atomic transaction.
- **`delete_article`** - Permanently delete an article and all of its content blocks by ID or slug.
- **`delete_content_block`** - Delete an individual content block from an article. Remaining blocks are automatically re-numbered sequentially and the article's featured image is re-calculated.
- **`get_article`** - Retrieve a single article and all of its ordered content blocks by ID or slug.
- **`list_articles`** - List and search MacronCMS articles with pagination, metadata, and optional full content blocks.
- **`list_content_types`** - List all available MacronCMS widget content types (e.g. heading, markdown, image, embed, three_js_quote), their fields, accepted dropdown options, convertible types, and featured image bubbling flags.
- **`reorder_content_blocks`** - Reorder content blocks within an article, either by specifying an explicit ordered ID list, or by moving a single block by position (1..N) or direction ('up' / 'down').
- **`replace_article_blocks`** - Replace the entire content block sequence of an article in one atomic transaction. To preserve existing file attachments (e.g. uploaded images), pass the existing block `id`.
- **`update_article_metadata`** - Update an article's metadata (title, slug, publication date, SEO tags, colors, background options, or background image) without modifying its content blocks.
- **`update_content_block`** - Update an individual content block's payload or file attachment without affecting other blocks in the article. Existing payload fields are preserved and merged by default.

---

## macronx

**Total Tools:** 7

- **`archive_inbox`** - Archive a processed or reviewed MacronX inbox entry by numeric ID.
- **`create_inbox`** - Ingest a new raw intelligence artifact or note into MacronX. Supports tags, JSON metadata, and file uploads (local files, remote URLs, or inline data). Assigning a tag linked to a MacronX workflow triggers automatic background analysis.
- **`get_inbox`** - Retrieve complete details for a single MacronX inbox entry by numeric ID, including full body, metadata, and attachment download links.
- **`get_inbox_attachment`** - Inspect, read, or download a file attachment from an inbox entry (e.g. IMINT imagery, audio intercept, PDF, or text). Returns native MCP image content for visual models, inline text for documents, or saves binary assets directly to disk.
- **`list_inboxes`** - List, search, filter, and paginate MacronX inbox items. By default returns active (unarchived) items with compact body previews to conserve context window.
- **`list_tags`** - List all MacronX intelligence tags available for inbox classification and workflow routing.
- **`unarchive_inbox`** - Restore an archived MacronX inbox entry back to the active inbox by numeric ID.

---

## mcp-motion

**Total Tools:** 30

- **`add_dots`** - Add colored dots at specific positions. Use for scatter plots, point highlights, or decorative elements.
- **`beat_add`** - Append a named beat. Idempotent on identical (name, hint, depends_on).
- **`beat_remove`** - Remove a beat by name. Fails if any directive references it.
- **`canvas_create`** - Create a new canvas session for drawing. Optionally load a question image with OCR text. If you skip this, a default session is auto-created on the first draw call.
- **`circle_text`** - Draw a circle around text to emphasize it. Use for the final answer, key conclusions, or important results. The reference must match text visible in the question (OCR).
- **`clear_canvas`** - Remove all drawings from the canvas. The question context is preserved.
- **`crossout_text`** - Draw a line through text to mark it as incorrect. Use for eliminating wrong answer choices, correcting errors, or showing process of elimination. The reference must match text visible in the question (OCR).
- **`directive_add`** - Append an L1 directive (emphasize/reveal/hide/compare/zoom_to/morph/annotate/reject) bound to a beat.
- **`directive_remove`** - Remove a directive by its id (or by index if id absent).
- **`display_text`** - Display non-math text on the canvas (titles, labels, descriptions, bullet points).
- **`draw_coordinate_system`** - Draw an x-y coordinate system with axes, labels, and optional grid. Use before plot_function.
- **`draw_shape`** - Draw a geometric shape (rectangle, ellipse, line, polygon) on the canvas.
- **`edit_patch`** - General editing primitive. Apply an arbitrary JSON Patch to a scene under optimistic concurrency (revision token). All other mutating tools compile to calls of this.
- **`finalize_answer`** - Highlight the correct answer and cross out all incorrect options. Use at the end of a multiple-choice question session.
- **`get_canvas`** - Get the current canvas state including all steps, animation JSON, and a visual preview.
- **`highlight_text`** - Highlight text in the question image to draw attention to important information. The reference must match text visible in the question (OCR). Use for key numbers, variables, conditions, or formulas.
- **`object_add`** - Add an L0 primitive to a scene. Returns the new revision and the JSON Patch that was applied.
- **`object_remove`** - Remove an object from a scene. Will fail if any directive still references it.
- **`object_update`** - Replace an existing object. Use object_remove to delete.
- **`page_switch`** - Clear the canvas and start a new page. Use when starting a new topic or when the canvas is full.
- **`plot_function`** - Plot a function on the coordinate system. Call draw_coordinate_system first. Expression uses JavaScript math (Math.sin, Math.pow, etc.).
- **`plot_line`** - Draw a line or polyline connecting points on the canvas. Use for graphs, arrows, connections.
- **`scene_create`** - Create a new empty scene. Returns the scene id and revision.
- **`scene_describe`** - Natural-language summary of a scene (title, beats, directives, objects).
- **`scene_get`** - Fetch the full scene by id.
- **`scene_list`** - List all known scenes with id, title, revision, last-updated.
- **`scene_preview`** - Render a terminal-friendly visual preview of the scene: canvas with objects, animation timeline with beat durations, and compiled L0 command summary. Use this after scene_render to show the result in the terminal.
- **`scene_render`** - Compile the scene to L0 MotionShark commands. v0.1 reference returns the compiled AnimationJSON; a full pixel render requires the MotionShark backend adapter.
- **`scene_validate`** - Run schema + cross-reference + beat-cycle validation. Returns ok or structured error.
- **`write_tex`** - Write a mathematical expression or equation on the canvas using LaTeX. Use this for every math step: definitions, substitutions, simplifications, final answers. Do NOT narrate the writing action in speech — the student sees the board.

---

## memorable

**Total Tools:** 17

- **`memorable_append_to_memory`** - Safely append Markdown content to an existing memory without overwriting its prior body
- **`memorable_create_memory`** - Create a new memory in Memorable (automatically enqueues vector embedding in the background)
- **`memorable_delete_attachment`** - Purge and delete an attachment from a memory
- **`memorable_delete_memory`** - Permanently delete a memory and its associated attachments from Memorable
- **`memorable_find_neighbors`** - Find nearest semantic neighbor memories via 1024-dimensional pgvector cosine distance
- **`memorable_generate_embedding`** - Generate or refresh the 1024-dimensional vector embedding for a memory using Ollama (synchronous or async background job)
- **`memorable_get_memory`** - Retrieve a memory's full Markdown content, embedding status, attachments, and optional rendered HTML
- **`memorable_get_stats`** - Get system statistics from Memorable (total memories, pinned memories, and attachments count)
- **`memorable_list_attachments`** - List file attachments and download URLs associated with a memory
- **`memorable_list_memories`** - List, filter, and paginate memories in Memorable with optional query, mode, and pinned filters
- **`memorable_recall_context`** - Recalls standing pinned memories combined with relevant semantic search matches in one unified context payload
- **`memorable_render_markdown`** - Render Markdown text to sanitized HTML using Memorable's Redcarpet GitHub-flavored markdown pipeline
- **`memorable_reorder_pinned`** - Update the sequential order of pinned memories displayed at the top of the Memorable workspace
- **`memorable_search`** - Unified vector and keyword search across Memorable memories using pgvector cosine similarity or text matching
- **`memorable_toggle_pin`** - Toggle the pinned status of a memory in the Memorable workspace
- **`memorable_update_memory`** - Update a memory's title, Markdown body, or pinned status in Memorable
- **`memorable_upload_attachment`** - Upload one or more files to attach to a memory in Memorable (accepts local file paths or base64 data)

---

## noteking

**Total Tools:** 18

- **`noteking_append_to_note`** - Safely append a Markdown section or log entry to the end of an existing note without overwriting its prior body
- **`noteking_create_note`** - Create a new Markdown note in NoteKing (under a project or as a standalone scratchpad note)
- **`noteking_create_project`** - Create a new note project workspace in NoteKing
- **`noteking_delete_attachment`** - Purge and delete an attachment from a note
- **`noteking_delete_note`** - Permanently delete a note and its attachments from NoteKing
- **`noteking_delete_project`** - Delete a project from NoteKing (notes belonging to this project are preserved as standalone notes)
- **`noteking_get_note`** - Retrieve a note's full Markdown content, metadata, attachments, and optional rendered HTML
- **`noteking_get_project`** - Get full project details including its associated note list index and metadata
- **`noteking_get_stats`** - Get system statistics from NoteKing (total notes, standalone notes, pinned notes, projects, and attachments)
- **`noteking_list_attachments`** - List file attachments associated with a note
- **`noteking_list_notes`** - List, filter, and search notes in NoteKing by full-text query, project, standalone scope, or pinned status
- **`noteking_list_projects`** - List and search note projects / workspaces in NoteKing with note count metrics and pagination
- **`noteking_render_markdown`** - Render Markdown text to sanitized HTML using NoteKing's GitHub-flavored markdown pipeline
- **`noteking_reorder_pinned`** - Update the sequential order of pinned notes displayed in the NoteKing sidebar
- **`noteking_toggle_pin`** - Toggle the pinned status of a note on the NoteKing sidebar
- **`noteking_update_note`** - Update a note's title, Markdown body, project assignment, or pinned status
- **`noteking_update_project`** - Update an existing project's name or description in NoteKing
- **`noteking_upload_attachment`** - Upload one or more files to attach to a note in NoteKing (accepts local file paths or base64 data)

---

## physicist

**Total Tools:** 51

- **`compute_clusters`** - Compute live connected-components vector clusters for SubatomicParticles or QuantumStates across particle groups without modifying the database.
- **`create_cluster_report`** - Initiate a 2-Phase Map-Reduce synthesis report on a frozen cluster snapshot.
- **`create_cluster_snapshot`** - Compute connected-components clustering and freeze it immediately into an immutable database snapshot.
- **`create_particle_group`** - Create a new particle group record in the catalog.
- **`create_quantum_state`** - Create a new quantum state or eigenmode under a subatomic particle.
- **`create_subatomic_particle`** - Create a new subatomic particle record in Physicist.
- **`delete_cluster_report`** - Delete a cluster report and its intermediate summaries.
- **`delete_cluster_snapshot`** - Delete a frozen cluster snapshot along with its cascaded cluster groups and synthesis reports.
- **`delete_particle_group`** - Delete a particle group and its cascaded subatomic particles and quantum states.
- **`delete_quantum_state`** - Delete a quantum state from the catalog.
- **`delete_subatomic_particle`** - Delete a subatomic particle and its cascaded quantum states.
- **`find_counterparts`** - Find nearest physical counterparts or symmetry analogs to a specified subatomic particle or quantum state using 1024-dimensional pgvector cosine distance.
- **`generate_deep_synthesis`** - Upgrade or run a 3-Phase Hierarchical Deep Synthesis report over a cluster snapshot with intermediate batch aggregation.
- **`generate_quantum_state_embedding`** - Generate or regenerate a 1024-dimensional semantic embedding vector for a quantum state.
- **`generate_subatomic_particle_embedding`** - Generate or regenerate a 1024-dimensional semantic embedding vector for a single subatomic particle.
- **`get_cluster_group`** - Retrieve details of a specific archetype cluster group with all member subatomic particles or quantum states.
- **`get_cluster_report`** - Retrieve complete scholarly physics report content, progress percentage, markdown monograph, and intermediate summaries.
- **`get_cluster_snapshot`** - Retrieve details of a frozen cluster snapshot including member groups and generated synthesis reports.
- **`get_job_status`** - Check the status, progress, and result of an ActiveJob/Sidekiq background task.
- **`get_openapi_spec`** - Retrieve the raw OpenAPI 3.1 specification for the Physicist API.
- **`get_particle_group`** - Retrieve details of a single particle group including its subatomic particles.
- **`get_platform_status`** - Get overall platform health, catalog entity counts, embedding coverage stats, and active LLM configuration.
- **`get_quantum_state`** - Retrieve details of a single quantum state including parent subatomic particle and particle group metadata.
- **`get_report_sub_report`** - Retrieve a single Phase 2 batch analysis.
- **`get_report_summary`** - Retrieve a single Phase 1 per-cluster scholarly summary.
- **`get_settings`** - Get embedding completion metrics for SubatomicParticles and QuantumStates, active embedding/LLM parameters, and context window presets.
- **`get_subatomic_particle`** - Retrieve details of a single subatomic particle including its particle group and child quantum states.
- **`list_cluster_groups`** - List all archetype cluster groups belonging to a specific frozen snapshot.
- **`list_cluster_reports`** - List generated multi-phase comparative particle physics and quantum state manifold synthesis reports.
- **`list_cluster_snapshots`** - List frozen archetype cluster snapshots in Physicist.
- **`list_jobs`** - List recent asynchronous background jobs (embedding calculations, LLM discoveries, synthesis reports).
- **`list_particle_groups`** - List particle groups (taxonomic families, structural sectors, supermultiplets) registered in Physicist with subatomic particle counts.
- **`list_quantum_states`** - List quantum states and eigenmodes registered in Physicist with filtering by subatomic particle, particle group, themes, and embedding status.
- **`list_report_sub_reports`** - List all Phase 2 intermediate batch analyses belonging to a detailed synthesis report.
- **`list_report_summaries`** - List all Phase 1 per-cluster analyses belonging to a synthesis report.
- **`list_subatomic_particles`** - List subatomic particles registered in Physicist with filtering by particle group, themes, embedding status, and search keywords.
- **`populate_particle_group_subatomic_particles`** - Discover and populate subatomic particles for a specific particle group via LLM generation.
- **`populate_particle_groups`** - Trigger LLM discovery to populate major particle groups and families with physics descriptions.
- **`populate_quantum_states_bulk`** - Bulk trigger discovery of quantum states across all subatomic particles under an optional subatomic particle scope.
- **`populate_subatomic_particle_quantum_states`** - Discover and populate quantum states, eigenmodes, and helicity manifolds for a subatomic particle via LLM analysis.
- **`populate_subatomic_particles_bulk`** - Bulk trigger discovery of subatomic particles across one or all particle groups via background job.
- **`search`** - Unified cross-catalog semantic or keyword search across subatomic particles and quantum states in the Physicist comparative physics manifold.
- **`trigger_bulk_embeddings`** - Enqueue bulk embedding generation for all SubatomicParticles or QuantumStates.
- **`update_context_window`** - Dynamically update the active LLM context window token size.
- **`update_particle_group`** - Update an existing particle group's name or description.
- **`update_quantum_state`** - Update an existing quantum state's attributes.
- **`update_subatomic_particle`** - Update an existing subatomic particle's attributes.
- **`upsert_particle_groups_batch`** - Batch insert or update particle groups matching case-insensitively on name.
- **`upsert_quantum_states_batch`** - Batch insert or update quantum states for a specific subatomic particle matching on lower(name).
- **`upsert_subatomic_particles_batch`** - Batch insert or update subatomic particles under a specific particle group matching on lower(name).
- **`wait_for_job`** - Poll a background job until completion or failure with configurable timeout.

---

## statesman

**Total Tools:** 51

- **`compute_clusters`** - Compute live connected-components vector clusters for Countries or Cities across continents without modifying the database.
- **`create_city`** - Create a new strategic city record associated with a sovereign country.
- **`create_cluster_report`** - Initiate a 2-Phase Map-Reduce synthesis report on a frozen cluster snapshot.
- **`create_cluster_snapshot`** - Compute connected-components clustering and freeze it immediately into an immutable database snapshot.
- **`create_continent`** - Create a new continent record in the catalog.
- **`create_country`** - Create a new sovereign country record associated with a continent.
- **`delete_city`** - Delete a city record.
- **`delete_cluster_report`** - Delete a synthesis report along with its intermediate summaries and sub-reports.
- **`delete_cluster_snapshot`** - Delete a frozen cluster snapshot along with its cascaded cluster groups and synthesis reports.
- **`delete_continent`** - Delete a continent and its cascaded countries and cities.
- **`delete_country`** - Delete a country and its cascaded strategic cities.
- **`find_counterparts`** - Find nearest geopolitical or urban counterparts to a specified country or city using 1024-dimensional pgvector cosine distance.
- **`generate_city_embedding`** - Calculate 1024-dimensional vector embedding for a city record.
- **`generate_country_embedding`** - Calculate 1024-dimensional vector embedding for a country using the configured embedding model.
- **`generate_deep_synthesis`** - Initiate a 3-Phase Hierarchical Deep Synthesis monograph, reusing Phase 1 summaries from a completed parent report.
- **`get_city`** - Retrieve details of a strategic city including its structured themes and associated country/continent.
- **`get_cluster_group`** - Retrieve details of a specific archetype cluster group with all member countries or cities.
- **`get_cluster_report`** - Retrieve complete scholarly report content, progress percentage, markdown monograph, and intermediate summaries.
- **`get_cluster_snapshot`** - Retrieve details of a frozen cluster snapshot including member groups and generated reports.
- **`get_continent`** - Retrieve details of a single continent including its sovereign countries.
- **`get_country`** - Retrieve full profile of a sovereign country including continent, thematic statecraft tags, and strategic cities.
- **`get_job_status`** - Check the status, progress, and result of an ActiveJob/Sidekiq background task.
- **`get_openapi_spec`** - Retrieve the raw OpenAPI 3.1 specification for the Statesman API.
- **`get_platform_status`** - Get overall platform health, catalog entity counts, embedding coverage stats, and active LLM configuration.
- **`get_report_sub_report`** - Retrieve a single Phase 2 batch analysis.
- **`get_report_summary`** - Retrieve a single Phase 1 per-cluster scholarly summary.
- **`get_settings`** - Get embedding completion metrics for Countries and Cities, active embedding/LLM parameters, and context window presets.
- **`list_cities`** - List and filter strategic urban power centers with civic/economic themes and embedding metadata.
- **`list_cluster_groups`** - List all archetype cluster groups belonging to a specific frozen snapshot.
- **`list_cluster_reports`** - List generated multi-phase comparative geopolitics and urban power synthesis reports.
- **`list_cluster_snapshots`** - List frozen archetype cluster snapshots.
- **`list_continents`** - List world continents registered in Statesman with sovereign country counts.
- **`list_countries`** - List and filter sovereign countries with statecraft themes, city counts, and vector embedding status.
- **`list_jobs`** - List recent asynchronous background jobs (embedding calculations, LLM discoveries, synthesis reports).
- **`list_report_sub_reports`** - List all Phase 2 intermediate batch analyses belonging to a detailed synthesis report.
- **`list_report_summaries`** - List all Phase 1 per-cluster analyses belonging to a synthesis report.
- **`populate_cities_bulk`** - Trigger bulk LLM city discovery across all countries or a single country.
- **`populate_continent_countries`** - Discover and populate sovereign countries for a specific continent via LLM generation.
- **`populate_continents`** - Trigger LLM discovery to populate all 7 standard continents with geopolitical descriptions.
- **`populate_countries_bulk`** - Trigger bulk LLM country discovery across all continents or a single continent.
- **`populate_country_cities`** - Discover and generate 8-10 strategic cities for a country via LLM extraction.
- **`search`** - Unified cross-catalog semantic or keyword search across sovereign countries and strategic cities in the Statesman comparative geopolitics manifold.
- **`trigger_bulk_embeddings`** - Enqueue bulk embedding generation for all Countries or Cities.
- **`update_city`** - Update an existing city's attributes, country, or thematic tags.
- **`update_context_window`** - Dynamically update the active LLM context window token size.
- **`update_continent`** - Update an existing continent's name or description.
- **`update_country`** - Update an existing country's attributes, continent, or thematic tags.
- **`upsert_cities_batch`** - Batch insert or update strategic cities scoped to a specific country.
- **`upsert_continents_batch`** - Batch insert or update continents matching case-insensitively on name.
- **`upsert_countries_batch`** - Batch insert or update sovereign countries scoped to a specific continent.
- **`wait_for_job`** - Poll a background job until completion or failure with configurable timeout.

---

## syncretica

**Total Tools:** 46

- **`compute_clusters`** - Compute live connected-components vector clusters for Gods or Myths across world pantheons without modifying the database.
- **`create_cluster_report`** - Initiate a 2-Phase Map-Reduce synthesis report on a frozen cluster snapshot.
- **`create_cluster_snapshot`** - Compute connected-components clustering and freeze it immediately into an immutable database snapshot.
- **`create_god`** - Create a new deity record associated with a pantheon.
- **`create_myth`** - Create or upsert a myth proposition record for a deity.
- **`create_pantheon`** - Create a new pantheon record in the catalog.
- **`delete_cluster_snapshot`** - Delete a frozen cluster snapshot along with its cascaded cluster groups and synthesis reports.
- **`delete_god`** - Delete a deity and its associated myth record.
- **`delete_myth`** - Delete a myth record.
- **`delete_pantheon`** - Delete a pantheon and its cascaded deities and myths.
- **`find_counterparts`** - Find nearest mythological counterparts to a specified god or myth using pgvector cosine distance across world pantheons.
- **`generate_deep_synthesis`** - Initiate a 3-Phase Hierarchical Deep Synthesis monograph, reusing Phase 1 summaries from a completed parent report.
- **`generate_god_embedding`** - Calculate 1024-dimensional vector embedding for a deity using the configured embedding model.
- **`generate_myth_embedding`** - Calculate 1024-dimensional vector embedding for a myth record.
- **`get_cluster_group`** - Retrieve details of a specific archetype cluster group with all member deities or myths.
- **`get_cluster_report`** - Retrieve complete scholarly report content, progress percentage, markdown monograph, and intermediate summaries.
- **`get_cluster_snapshot`** - Retrieve details of a frozen cluster snapshot including member groups and generated reports.
- **`get_god`** - Retrieve full profile of a deity including pantheon, thematic attributes, and myth propositions.
- **`get_job_status`** - Check the status, progress, and result of an ActiveJob/Sidekiq background task.
- **`get_myth`** - Retrieve details of a myth including its 8-10 decomposed themes and associated deity.
- **`get_openapi_spec`** - Retrieve the raw OpenAPI 3.1 specification for the Syncretica API.
- **`get_pantheon`** - Retrieve details of a single pantheon including its deity roster.
- **`get_platform_status`** - Get overall platform health, catalog entity counts, embedding coverage stats, and active LLM configuration.
- **`get_report_sub_report`** - Retrieve a single Phase 2 batch analysis.
- **`get_report_summary`** - Retrieve a single Phase 1 per-cluster scholarly summary.
- **`get_settings`** - Get embedding completion metrics, active embedding/LLM parameters, and context window presets.
- **`list_cluster_reports`** - List generated multi-phase comparative mythology reports and monographs.
- **`list_cluster_snapshots`** - List frozen archetype cluster snapshots.
- **`list_gods`** - List and filter deities with thematic tags and vector embedding status.
- **`list_jobs`** - List recent asynchronous background jobs (embedding calculations, LLM discoveries, synthesis reports).
- **`list_myths`** - List and filter mythologies with structured propositions and embedding metadata.
- **`list_pantheons`** - List world mythological pantheons registered in Syncretica with deity counts.
- **`populate_god_myth`** - Generate 8-10 structured mythological themes for a deity via LLM extraction.
- **`populate_gods_bulk`** - Trigger bulk LLM discovery across all or a single pantheon.
- **`populate_myths_bulk`** - Trigger bulk myth discovery across all deities or a single deity.
- **`populate_pantheon_gods`** - Discover and populate deities for a specific pantheon via LLM generation.
- **`populate_pantheons`** - Trigger LLM discovery to identify and populate global pantheons.
- **`search`** - Unified cross-catalog semantic or keyword search across deities and myths in the Syncretica comparative mythology manifold.
- **`trigger_bulk_embeddings`** - Enqueue bulk embedding generation for all Gods or Myths.
- **`update_context_window`** - Dynamically update the active LLM context window token size.
- **`update_god`** - Update an existing deity's attributes, pantheon, or thematic tags.
- **`update_myth`** - Update an existing myth's structured theme propositions.
- **`update_pantheon`** - Update an existing pantheon's name or description.
- **`upsert_gods_batch`** - Batch insert or update deities scoped to a specific pantheon.
- **`upsert_pantheons_batch`** - Batch insert or update pantheons matching case-insensitively on name.
- **`wait_for_job`** - Poll a background job until completion or failure with configurable timeout.

---

## wikidata

**Total Tools:** 7

- **`check_health`** - Verify connectivity to the local QLever Wikidata Truthy SPARQL endpoint and return the total indexed triple count and query latency.
- **`find_cross_links`** - Discover direct relationships and shared hubs (alliances, conflicts, parent entities, shared bodies of water) between a set of resolved Wikidata entities, filtering out irrelevant entertainment/sports hubs.
- **`get_entity_triples`** - Retrieve curated outbound Wikidata triples for one or more entity QIDs. Returns grouped, deduplicated facts with human-readable predicate and object labels.
- **`get_inbound_relations`** - Retrieve inbound relations for target entities (e.g. alliance members via P463, conflict participants via P710, basin countries via P205, corporate owners via P127). Includes accurate total counts and truncation flags.
- **`ground_entities`** - Single composite tool to ground a brief: resolves all mentions to Wikidata QIDs, retrieves curated outbound triples, discovers inter-entity cross-links and shared hubs, and retrieves key inbound rosters.
- **`query_sparql`** - Execute an arbitrary read-only SPARQL SELECT or ASK query against the local QLever Wikidata endpoint. Auto-declares standard prefixes (wd:, wdt:, rdfs:, xsd:) and enforces query limits.
- **`resolve_entities`** - Resolve a batch of named entity mentions to Wikidata QIDs using deterministic label matching, domain P31/P279 class filtering, homonym scoring, and disambiguation fingerprints.

---

## Additional Configured Remote MCP Endpoints

The following servers are configured as remote SSE endpoints in `~/.gemini/config/mcp_config.json` with dynamic runtime schemas:

- **`hyperframes`** - `https://mcp.heygen.com/mcp/hyperframes/`
