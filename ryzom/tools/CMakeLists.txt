ADD_SUBDIRECTORY(skill_extractor)
ADD_SUBDIRECTORY(make_alias_file)
ADD_SUBDIRECTORY(make_anim_by_race)
ADD_SUBDIRECTORY(make_anim_melee_impact)
ADD_SUBDIRECTORY(pd_parser)
ADD_SUBDIRECTORY(translation_tools)
ADD_SUBDIRECTORY(assoc_mem)
ADD_SUBDIRECTORY(leveldesign)
ADD_SUBDIRECTORY(patch_gen)
ADD_SUBDIRECTORY(pdr_util)
ADD_SUBDIRECTORY(stats_scan)

IF(WITH_RYZOM_CLIENT)
  ADD_SUBDIRECTORY(sheets_packer) 
  ADD_SUBDIRECTORY(client)
ENDIF(WITH_RYZOM_CLIENT)

IF(WITH_RYZOM_SERVER)
  ADD_SUBDIRECTORY(server)
ENDIF(WITH_RYZOM_SERVER)

# Old stuff that doesn't compile anymore.
#ADD_SUBDIRECTORY(occ2huff)
#ADD_SUBDIRECTORY(phrase_generator)
#ADD_SUBDIRECTORY(sheet_random_generator)

# Not building these
#xml_packer - this is in NeL tools.

# Folders with nothing to build
#data_tools
#translation
#test_files
#build_data

# Folders with subfolders, TODO
#client

# folders not handled yet.
#connection_stats
#reynolds
