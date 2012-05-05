#==============================================================================#
#                                                                              #
#  Copyright (c) 2012 MaidSafe.net limited                                     #
#                                                                              #
#  The following source code is property of MaidSafe.net limited and is not    #
#  meant for external use.  The use of this code is governed by the license    #
#  file licence.txt found in the root directory of this project and also on    #
#  www.maidsafe.net.                                                           #
#                                                                              #
#  You are not free to copy, amend or otherwise use this source code without   #
#  the explicit written permission of the board of directors of MaidSafe.net.  #
#                                                                              #
#==============================================================================#


set(HR "================================================================================")
message("${HR}\nConfiguring third party projects\n--------------------------------\n")

add_subdirectory(cryptopp)
add_subdirectory(glog)
add_subdirectory(googlemock)
add_subdirectory(protobuf)

set(BUILD_PROJECTS date_time;filesystem;program_options;random;serialization;system;thread;)  # test
add_subdirectory(boost)