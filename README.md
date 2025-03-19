#//
//  ContentView.swift
//  DemoRecatngle
//
//  Created by Tony on 2025/3/18.
//

import SwiftUI

struct ContentView: View {
    var body: some View {
       ZStack {
           Color.aaa
               .ignoresSafeArea()
           Rectangle()//脖子
               .frame(width: 80, height: 100)
               .offset(y: 120)
               .foregroundColor(.brown)
           RoundedRectangle(cornerRadius: 50 )//臉
               .frame(width: 300, height: 200)
               .foregroundColor(.brown)
           RoundedRectangle(cornerRadius: 70)//衣服
               .frame(width: 350, height: 500)
               .offset(y: 400)
               .foregroundColor(Color(red: 160/255, green: 173/255, blue: 193/255))
           Text("Dodgers")
               .font(.system(size: 60, weight: .bold))
               .foregroundColor(.white)
               .offset(x: -130, y: 230 )
               .rotationEffect(.degrees(-25))
           Text("17")
               .font(.system(size: 60, weight: .bold))
               .foregroundColor(.white)
               .offset(x: 90, y: 300 )
           RoundedRectangle(cornerRadius: 70)//帽子
               .trim(from: 0.5, to: 1)
               .frame(width: 320, height: 320)
               .offset(y: -50)
               .foregroundStyle(Color(red: 7/255, green: 77/255, blue: 184/255))
           Capsule()//帽沿
               .frame(width: 350, height: 30)
               .offset(y: -50)
               .foregroundStyle(Color(red: 7/255, green: 77/255, blue: 184/255))
           Circle()//左眼
               .frame(width: 45)
               .offset(x: -75, y: 0)
           Circle()//右眼
               .frame(width: 45)
               .offset(x: 75, y: 0)
           Ellipse()//鼻子
               .frame(width: 20, height: 20)
               .offset(y: 30)
               .foregroundColor(.black.opacity(0.5))
           Capsule()//左眉毛
               .frame(width: 60, height: 10)
               .offset(x: -75, y: -30)
               .foregroundColor(.black)
           Capsule()//右眉毛
               .frame(width: 60, height: 10)
               .offset(x: 75, y: -30)
               .foregroundColor(.black)
           Text("L")
               .font(.custom("L", size: 90))
               .foregroundStyle(.white)
               .offset(x: -10, y: -140)
           Text("A")
               .font(.custom("L", size: 90))
               .foregroundStyle(.white)
               .offset(x: 12, y: -120)
           
        }

    }
        
    }

#Preview {
    ContentView()
}
