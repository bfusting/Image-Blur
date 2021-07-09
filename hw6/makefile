CFLAGS=
cudaBlur: ./fastblur.o
	nvcc $(CFLAGS) ./fastblur.o -o cudaBlur -lm


./fastblur.o: cudaBlur.cu
	nvcc -c $(CFLAGS) cudaBlur.cu -o ./fastblur.o 


clean:
	rm -f ./* cudaBlur output.png
