# Copyright 2023 MongoDB Inc.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
# http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/
    DESTINATION ${CMAKE_INSTALL_INCLUDEDIR}
    COMPONENT dev
    FILES_MATCHING PATTERN "*.hpp"
)

set_dist_list(src_mongocxx_include_DIST
    CMakeLists.txt
    mongocxx/v_noabi/mongocxx/bulk_write.hpp
    mongocxx/v_noabi/mongocxx/change_stream.hpp
    mongocxx/v_noabi/mongocxx/client_encryption.hpp
    mongocxx/v_noabi/mongocxx/client_session.hpp
    mongocxx/v_noabi/mongocxx/client.hpp
    mongocxx/v_noabi/mongocxx/collection.hpp
    mongocxx/v_noabi/mongocxx/config/compiler.hpp
    mongocxx/v_noabi/mongocxx/config/postlude.hpp
    mongocxx/v_noabi/mongocxx/config/prelude.hpp
    mongocxx/v_noabi/mongocxx/cursor.hpp
    mongocxx/v_noabi/mongocxx/database.hpp
    mongocxx/v_noabi/mongocxx/events/command_failed_event.hpp
    mongocxx/v_noabi/mongocxx/events/command_started_event.hpp
    mongocxx/v_noabi/mongocxx/events/command_succeeded_event.hpp
    mongocxx/v_noabi/mongocxx/events/heartbeat_failed_event.hpp
    mongocxx/v_noabi/mongocxx/events/heartbeat_started_event.hpp
    mongocxx/v_noabi/mongocxx/events/heartbeat_succeeded_event.hpp
    mongocxx/v_noabi/mongocxx/events/server_changed_event.hpp
    mongocxx/v_noabi/mongocxx/events/server_closed_event.hpp
    mongocxx/v_noabi/mongocxx/events/server_description.hpp
    mongocxx/v_noabi/mongocxx/events/server_opening_event.hpp
    mongocxx/v_noabi/mongocxx/events/topology_changed_event.hpp
    mongocxx/v_noabi/mongocxx/events/topology_closed_event.hpp
    mongocxx/v_noabi/mongocxx/events/topology_description.hpp
    mongocxx/v_noabi/mongocxx/events/topology_opening_event.hpp
    mongocxx/v_noabi/mongocxx/exception/authentication_exception.hpp
    mongocxx/v_noabi/mongocxx/exception/bulk_write_exception.hpp
    mongocxx/v_noabi/mongocxx/exception/error_code.hpp
    mongocxx/v_noabi/mongocxx/exception/exception.hpp
    mongocxx/v_noabi/mongocxx/exception/gridfs_exception.hpp
    mongocxx/v_noabi/mongocxx/exception/logic_error.hpp
    mongocxx/v_noabi/mongocxx/exception/operation_exception.hpp
    mongocxx/v_noabi/mongocxx/exception/query_exception.hpp
    mongocxx/v_noabi/mongocxx/exception/server_error_code.hpp
    mongocxx/v_noabi/mongocxx/exception/write_exception.hpp
    mongocxx/v_noabi/mongocxx/gridfs/bucket.hpp
    mongocxx/v_noabi/mongocxx/gridfs/downloader.hpp
    mongocxx/v_noabi/mongocxx/gridfs/uploader.hpp
    mongocxx/v_noabi/mongocxx/hint.hpp
    mongocxx/v_noabi/mongocxx/index_model.hpp
    mongocxx/v_noabi/mongocxx/index_view.hpp
    mongocxx/v_noabi/mongocxx/instance.hpp
    mongocxx/v_noabi/mongocxx/logger.hpp
    mongocxx/v_noabi/mongocxx/model/delete_many.hpp
    mongocxx/v_noabi/mongocxx/model/delete_one.hpp
    mongocxx/v_noabi/mongocxx/model/insert_one.hpp
    mongocxx/v_noabi/mongocxx/model/replace_one.hpp
    mongocxx/v_noabi/mongocxx/model/update_many.hpp
    mongocxx/v_noabi/mongocxx/model/update_one.hpp
    mongocxx/v_noabi/mongocxx/model/write.hpp
    mongocxx/v_noabi/mongocxx/options/aggregate.hpp
    mongocxx/v_noabi/mongocxx/options/apm.hpp
    mongocxx/v_noabi/mongocxx/options/auto_encryption.hpp
    mongocxx/v_noabi/mongocxx/options/bulk_write.hpp
    mongocxx/v_noabi/mongocxx/options/change_stream.hpp
    mongocxx/v_noabi/mongocxx/options/client_encryption.hpp
    mongocxx/v_noabi/mongocxx/options/client_session.hpp
    mongocxx/v_noabi/mongocxx/options/client.hpp
    mongocxx/v_noabi/mongocxx/options/count.hpp
    mongocxx/v_noabi/mongocxx/options/create_collection.hpp
    mongocxx/v_noabi/mongocxx/options/data_key.hpp
    mongocxx/v_noabi/mongocxx/options/delete.hpp
    mongocxx/v_noabi/mongocxx/options/distinct.hpp
    mongocxx/v_noabi/mongocxx/options/encrypt.hpp
    mongocxx/v_noabi/mongocxx/options/estimated_document_count.hpp
    mongocxx/v_noabi/mongocxx/options/find_one_and_delete.hpp
    mongocxx/v_noabi/mongocxx/options/find_one_and_replace.hpp
    mongocxx/v_noabi/mongocxx/options/find_one_and_update.hpp
    mongocxx/v_noabi/mongocxx/options/find_one_common_options.hpp
    mongocxx/v_noabi/mongocxx/options/find.hpp
    mongocxx/v_noabi/mongocxx/options/gridfs/bucket.hpp
    mongocxx/v_noabi/mongocxx/options/gridfs/upload.hpp
    mongocxx/v_noabi/mongocxx/options/index_view.hpp
    mongocxx/v_noabi/mongocxx/options/index.hpp
    mongocxx/v_noabi/mongocxx/options/insert.hpp
    mongocxx/v_noabi/mongocxx/options/pool.hpp
    mongocxx/v_noabi/mongocxx/options/range.hpp
    mongocxx/v_noabi/mongocxx/options/replace.hpp
    mongocxx/v_noabi/mongocxx/options/rewrap_many_datakey.hpp
    mongocxx/v_noabi/mongocxx/options/server_api.hpp
    mongocxx/v_noabi/mongocxx/options/ssl.hpp
    mongocxx/v_noabi/mongocxx/options/tls.hpp
    mongocxx/v_noabi/mongocxx/options/transaction.hpp
    mongocxx/v_noabi/mongocxx/options/update.hpp
    mongocxx/v_noabi/mongocxx/pipeline.hpp
    mongocxx/v_noabi/mongocxx/pool.hpp
    mongocxx/v_noabi/mongocxx/read_concern.hpp
    mongocxx/v_noabi/mongocxx/read_preference.hpp
    mongocxx/v_noabi/mongocxx/result/bulk_write.hpp
    mongocxx/v_noabi/mongocxx/result/delete.hpp
    mongocxx/v_noabi/mongocxx/result/gridfs/upload.hpp
    mongocxx/v_noabi/mongocxx/result/insert_many.hpp
    mongocxx/v_noabi/mongocxx/result/insert_one.hpp
    mongocxx/v_noabi/mongocxx/result/replace_one.hpp
    mongocxx/v_noabi/mongocxx/result/rewrap_many_datakey.hpp
    mongocxx/v_noabi/mongocxx/result/update.hpp
    mongocxx/v_noabi/mongocxx/search_index_model.hpp
    mongocxx/v_noabi/mongocxx/search_index_view.hpp
    mongocxx/v_noabi/mongocxx/stdx.hpp
    mongocxx/v_noabi/mongocxx/uri.hpp
    mongocxx/v_noabi/mongocxx/validation_criteria.hpp
    mongocxx/v_noabi/mongocxx/write_concern.hpp
    mongocxx/v_noabi/mongocxx/write_type.hpp
)
