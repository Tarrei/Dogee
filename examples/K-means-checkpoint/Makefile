K-means-checkpoint: K-means-checkpoint.o
	$(CXX) -o $(BIN_DIR)/$@ $(CXXFLAGS) -Wl,--start-group $^ $(BIN_DIR)/libDogee.a $(LIBS) -Wl,--end-group 
.PHONY:clean
clean:
	# If .o does not exist, don't stop
	rm -f K-means-checkpoint.o 
	rm -f $(BIN_DIR)/K-means
remake: clean K-means-checkpoint
