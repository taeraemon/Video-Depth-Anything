




# Setup
git clone https://github.com/DepthAnything/Video-Depth-Anything

cd Video-Depth-Anything

source env/bin/activate

pip install -r requirements.txt

pip install pyyaml typeguard

bash get_weights.sh





# Run

python3 run.py --input_video ./assets/example_videos/davis_rollercoaster.mp4 --output_dir ./outputs --encoder vitl

python3 run_streaming.py --input_video ./assets/example_videos/davis_rollercoaster.mp4 --output_dir ./outputs_streaming --encoder vitl

python3 run_streaming.py --input_video ./assets/example_videos/Tokyo-Walk_rgb.mp4 --output_dir ./outputs_streaming --encoder vitl

python3 run_streaming.py --input_video ./assets/example_videos/helicopter_H_001.avi --output_dir ./outputs_streaming --encoder vitl

python3 run_streaming.py --input_video ./assets/example_videos/crowd_S_001.avi --output_dir ./outputs_streaming --encoder vitl


