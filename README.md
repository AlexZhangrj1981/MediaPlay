//音频
    [PlayModel shareInstance].playDelegate = self;
    [[PlayModel shareInstance] initAudioPlayerWithUrl:[NSURL URLWithString:@""]];
    
    //视频
    MoviePlayerViewController *movieplayer = [MoviePlayerViewController new];
    movieplayer.playUrl = @"";//远程视频
//    movieplayer.localUrl = [NSURL URLWithString:@""];//本地视频
    [self.navigationController pushViewController:movieplayer animated:YES];
