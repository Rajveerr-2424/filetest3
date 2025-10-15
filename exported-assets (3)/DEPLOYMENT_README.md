# Russian Roulette DApp - Vercel Deployment Guide

🎲 **Complete deployment-ready Russian Roulette blockchain game with Filecoin testnet integration**

## 📦 What's Included

This zip file contains a complete Next.js application ready for Vercel deployment:

- ✅ **Russian Roulette Game** with Player vs Bot mechanics
- ✅ **3D Graphics** using React Three Fiber
- ✅ **Filecoin Testnet Integration** (Chain ID: 314159)
- ✅ **MetaMask Wallet Connection**
- ✅ **Sound Effects System**
- ✅ **Responsive Design** for all devices
- ✅ **Production Optimizations**

## 🚀 Quick Deployment to Vercel

### Method 1: Drag & Drop (Easiest)
1. Go to [vercel.com](https://vercel.com)
2. Sign in or create account
3. Drag and drop this ZIP file onto the deployment area
4. Vercel will automatically deploy your app!

### Method 2: GitHub Integration
1. Extract ZIP to a new folder
2. Initialize git: `git init`
3. Create GitHub repository
4. Push code to GitHub
5. Connect repository to Vercel
6. Auto-deploy on every push

### Method 3: Vercel CLI
```bash
# Install Vercel CLI
npm i -g vercel

# Extract ZIP and navigate to folder
cd roulette-dapp-vercel

# Deploy
vercel --prod
```

## 🔧 Environment Configuration

After deployment, you'll need to update these environment variables in Vercel:

### Required Updates:
1. **NEXT_PUBLIC_CONTRACT_ADDRESS**: Update after deploying smart contract
2. **NEXT_PUBLIC_WALLET_CONNECT_PROJECT_ID**: Already configured
3. **NEXT_PUBLIC_CHAIN_ID**: Set to 314159 (Filecoin testnet)

### In Vercel Dashboard:
1. Go to your project settings
2. Navigate to "Environment Variables"
3. Update `NEXT_PUBLIC_CONTRACT_ADDRESS` with your deployed contract address

## 📋 Pre-configured Features

### Blockchain Integration
- **Network**: Filecoin Calibration Testnet (314159)
- **RPC**: https://api.calibration.node.glif.io/rpc/v1
- **Wallet**: MetaMask + WalletConnect support
- **Currency**: tFIL (test Filecoin)

### Game Features
- **6-Chamber Revolver** with random bullet placement
- **Player vs Bot** gameplay
- **Scoring System**: Death penalty (-10), Streak bonus (+20)
- **3D Animations** with React Three Fiber
- **Sound Effects** for immersive experience
- **Achievement System** with notifications

### UI/UX
- **Dark Gaming Theme** optimized for the Russian Roulette aesthetic
- **Responsive Design** works on mobile, tablet, desktop
- **Loading States** for all blockchain interactions
- **Error Handling** with user-friendly messages
- **Accessibility** features included

## 🎮 Game Flow

1. **Homepage**: Welcome screen with wallet connection
2. **Game Page**: Main 3D interface with revolver and characters
3. **Wallet Integration**: Connect MetaMask to Filecoin testnet
4. **Gameplay**: Choose to fire at self or bot
5. **Blockchain**: Smart contract determines random outcome
6. **Results**: Animated results with point updates
7. **Achievements**: Unlock rewards for milestones

## 📁 Project Structure

```
roulette-dapp-vercel/
├── app/                    # Next.js 14 App Router
│   ├── page.tsx           # Homepage
│   ├── game/page.tsx      # Main game interface
│   ├── leaderboard/page.tsx # Player statistics
│   └── layout.tsx         # Root layout
├── components/            # React components
│   ├── game/              # Game-specific components
│   ├── ui/                # UI components
│   └── web3/              # Blockchain components
├── lib/                   # Utility functions
├── hooks/                 # Custom React hooks
├── public/                # Static assets
└── styles/                # Styling files
```

## 🔗 After Deployment

### 1. Deploy Smart Contract
Use the provided Hardhat configuration to deploy the game contract to Filecoin testnet:
```bash
# In your smart contract folder
npm run deploy:filecoin
```

### 2. Update Contract Address
Update the `NEXT_PUBLIC_CONTRACT_ADDRESS` environment variable in Vercel with your deployed contract address.

### 3. Test the Game
1. Visit your deployed Vercel URL
2. Connect MetaMask wallet
3. Switch to Filecoin testnet
4. Play the game!

## 📱 Mobile Optimization

The app is fully responsive and optimized for:
- **iOS Safari** and **Chrome Mobile**
- **Touch Controls** for game interactions
- **Progressive Web App** capabilities
- **Offline Fallbacks** for better UX

## 🔧 Customization

### Adding 3D Models
1. Add `.glb` files to `/public/models/`
2. Update component imports
3. Redeploy

### Adding Sound Effects
1. Add `.mp3` files to `/public/sounds/`
2. Update sound configuration
3. Redeploy

### Styling Changes
- Edit TailwindCSS classes in components
- Modify `/styles/globals.css` for global styles
- Update theme colors in `/lib/constants.ts`

## 🌐 Production Features

- **Automatic HTTPS** via Vercel
- **Global CDN** for fast loading worldwide
- **Edge Functions** for optimal performance
- **Analytics** ready (add Vercel Analytics)
- **SEO Optimized** with proper meta tags

## 🔒 Security Notes

- All sensitive operations happen on-chain
- Private keys never leave user's wallet
- Environment variables properly scoped
- Input validation on all user inputs
- Rate limiting considerations

## 🆘 Troubleshooting

### Common Issues:
1. **Contract not found**: Update NEXT_PUBLIC_CONTRACT_ADDRESS
2. **Network errors**: Check Filecoin testnet RPC status
3. **Wallet connection**: Ensure MetaMask has Filecoin testnet added
4. **3D not loading**: Check WebGL support in browser

### Support Resources:
- Vercel Documentation: https://vercel.com/docs
- Next.js Documentation: https://nextjs.org/docs
- Filecoin Developer Resources: https://docs.filecoin.io

## 🎉 Success Metrics

After deployment, your app will have:
- ⚡ **Fast Loading**: < 3 seconds on average connection
- 📱 **Mobile Friendly**: Works on all devices
- 🔗 **Blockchain Ready**: Full Web3 integration
- 🎮 **Engaging UX**: Smooth 3D animations and sounds
- 🌍 **Global Reach**: CDN-powered worldwide access

## 📈 Next Steps

1. **Deploy to Vercel** (drag & drop the ZIP)
2. **Deploy smart contract** to Filecoin testnet
3. **Update environment variables** in Vercel
4. **Test thoroughly** on different devices
5. **Share with users** and gather feedback
6. **Monitor analytics** and optimize performance

Your Russian Roulette DApp is ready for the world! 🎲✨
