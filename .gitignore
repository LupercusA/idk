@@ -34,6 +34,7 @@ minetest.register_chatcommand("rank", {
	local param2 = param:split(' ')[2]
	local param3 = param:split(' ')[3]
	local player = minetest.get_player_by_name(param1)


		if not player then
			return
@@ -53,8 +54,8 @@ minetest.register_chatcommand("rank", {
			return
			minetest.chat_send_player(name, "Invaild rank color you can use red, blue, yellow, green, black, white") 
		end
		if param3 == "blue" or param3 == "red" or param3 == "yellow" or param3 == "green" or param3 == "black" or param3 == "white" and param2 ~= nil then
			player:set_nametag_attributes({text = ""..minetest.colorize(rank_color[player:get_attribute("rank_color")], player:get_attribute("rank_name")).."[ ]"..name})
		if param3 == "blue" or param3 == "red" or param3 == "yellow" or param3 == "green" or param3 == "black" or param3 == "white" and param2 ~= nil and player ~= nil then
			minetest.get_player_by_name(param1):set_nametag_attributes({text = ""..minetest.colorize(rank_color[player:get_attribute("rank_color")], player:get_attribute("rank_name")).." "..param1})
			minetest.chat_send_player(name, "Rank has been updated")
		end
	end
